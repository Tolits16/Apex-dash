# Git Commit Guide — Apex Dash
# Binary Lap Studios · 14-Day Sprint

This file is your cheat sheet for writing meaningful commits.
Each student needs 5+ commits. Use the messages below as a guide.
DO NOT copy-paste all at once — commit as you actually do the work.

═══════════════════════════════════════════════════════════════════
 STUDENT 1 — Lead Developer (Game Systems)
 Suggested commits spread across Day 1–13
═══════════════════════════════════════════════════════════════════

Day 1–2:
  git commit -m "init: set up repo structure and blank HTML5 canvas game file"

Day 3–4:
  git commit -m "feat(game): implement vehicle physics — acceleration, braking, turning"

Day 5–6:
  git commit -m "feat(game): add track geometry, grass boundary detection, and collision AABB"

Day 7–8:
  git commit -m "feat(game): implement speed boost pads and obstacle penalty system"

Day 9–10:
  git commit -m "feat(game): add ghost replay system with localStorage persistence"

Day 11:
  git commit -m "feat(game): implement sector checkpoints and finish line detection"

Day 12:
  git commit -m "fix(game): correct ghost frame timing and boost flame animation"

Day 13:
  git commit -m "polish(game): tune physics constants, add exhaust trail, improve HUD"

═══════════════════════════════════════════════════════════════════
 STUDENT 2 — UI/UX Developer (Web + Level Design)
 Suggested commits spread across Day 1–13
═══════════════════════════════════════════════════════════════════

Day 1–2:
  git commit -m "init: create index.html and team.html shells with base CSS variables"

Day 3–4:
  git commit -m "feat(site): build landing page hero section with animated grid background"

Day 5–6:
  git commit -m "feat(site): add game embed section with iframe, controls panel, and how-to-play"

Day 7–8:
  git commit -m "feat(site): complete team page — member cards, roles, GitHub links"

Day 9–10:
  git commit -m "feat(game): design track layout — obstacle placement and boost pad positions"

Day 11:
  git commit -m "feat(site): add features section, screenshots grid, and footer"

Day 12:
  git commit -m "fix(site): mobile responsive layout — nav, grid breakpoints, hero text scale"

Day 13:
  git commit -m "docs: complete README with screenshots, controls table, and sprint timeline"

═══════════════════════════════════════════════════════════════════
 SHARED — Either student can do these
═══════════════════════════════════════════════════════════════════

  git commit -m "chore: add .gitignore — exclude DS_Store and editor files"
  git commit -m "fix(game): cross-browser canvas rendering fix for Firefox"
  git commit -m "polish: update leaderboard display and sector time colours"
  git commit -m "docs: add screenshots to assets folder"

═══════════════════════════════════════════════════════════════════
 HOW TO COMMIT — Quick reference
═══════════════════════════════════════════════════════════════════

  git add .                          # Stage all changes
  git add game/index.html            # Stage a specific file
  git commit -m "your message here"  # Commit with a message
  git push origin main               # Push to GitHub

Commit message format used here:
  type(scope): short description

Types: feat, fix, polish, docs, chore, init
Scopes: game, site, docs

Examples of BAD commit messages (avoid these):
  "update"
  "fix stuff"
  "changes"
  "asdfgh"
  "final final FINAL v3"
