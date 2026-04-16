# Deploying Apex Dash to GitHub Pages
# Binary Lap Studios

Follow these steps exactly. Takes about 5 minutes.

───────────────────────────────────────────────────────────────────
 STEP 1 — Create the GitHub repository
───────────────────────────────────────────────────────────────────

1. Go to https://github.com and sign in (Student 1's account)
2. Click the "+" icon → "New repository"
3. Repository name: apex-dash
4. Set to: Public
5. DO NOT tick "Add a README" (we have our own)
6. Click "Create repository"

───────────────────────────────────────────────────────────────────
 STEP 2 — Add Student 2 as a collaborator
───────────────────────────────────────────────────────────────────

1. In your new repo, go to Settings → Collaborators
2. Click "Add people" → search for Student 2's GitHub username
3. Student 2 accepts the invite from their email or GitHub notifications

───────────────────────────────────────────────────────────────────
 STEP 3 — Push your files
───────────────────────────────────────────────────────────────────

Open your terminal / Git Bash in the apex-dash-site folder:

  git init
  git add .
  git commit -m "init: initial project structure — game, website, and README"
  git branch -M main
  git remote add origin https://github.com/YOURUSERNAME/apex-dash.git
  git push -u origin main

Replace YOURUSERNAME with your actual GitHub username.

───────────────────────────────────────────────────────────────────
 STEP 4 — Enable GitHub Pages
───────────────────────────────────────────────────────────────────

1. In your repo, go to Settings → Pages (left sidebar)
2. Under "Source", select: Deploy from a branch
3. Branch: main  |  Folder: / (root)
4. Click Save
5. Wait 1–2 minutes, then visit:
   https://YOURUSERNAME.github.io/apex-dash/

───────────────────────────────────────────────────────────────────
 STEP 5 — Verify everything works
───────────────────────────────────────────────────────────────────

Check these URLs work:
  https://YOURUSERNAME.github.io/apex-dash/           ← Landing page
  https://YOURUSERNAME.github.io/apex-dash/team.html  ← Team page
  https://YOURUSERNAME.github.io/apex-dash/game/      ← Game directly

If the game iframe shows a blank box on the landing page:
  → The game/index.html path is correct by default. 
  → Hard refresh with Ctrl+Shift+R or clear browser cache.

───────────────────────────────────────────────────────────────────
 STEP 6 — Update README and team.html with real links
───────────────────────────────────────────────────────────────────

In README.md:
  Replace: https://yourusername.github.io/apex-dash
  With:    your actual Pages URL

  Replace: github.com/yourusername  and  github.com/partnerusername
  With:    your real GitHub profile URLs

In team.html:
  Replace the placeholder [ Your Name ] and [ Partner Name ]
  Replace the github.com/yourusername href values

Commit these changes:
  git add .
  git commit -m "docs: update README and team page with real names and links"
  git push

───────────────────────────────────────────────────────────────────
 TROUBLESHOOTING
───────────────────────────────────────────────────────────────────

Problem: Pages shows a 404
Fix: Make sure index.html is in the ROOT folder, not inside a subfolder.
     The structure must be:  apex-dash/index.html  (not apex-dash/site/index.html)

Problem: Game doesn't load in the iframe
Fix: GitHub Pages serves over HTTPS. The iframe src="game/index.html" is 
     a relative path and works fine. If testing locally, use VS Code Live Server
     or: npx serve .

Problem: localStorage doesn't save between sessions
Fix: This is normal if you're viewing the file:// protocol.
     It works correctly when served from GitHub Pages (https://).

Problem: Font doesn't load
Fix: Google Fonts requires an internet connection. Works fine on GitHub Pages.
     For offline use, download and self-host the fonts.
