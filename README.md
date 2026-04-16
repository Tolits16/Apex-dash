# 🏎️ Apex Dash — Time Trial Racing

> A fast-paced, browser-based top-down time trial racer built with HTML5 Canvas and vanilla JavaScript.

**Binary Lap Studios** · 2nd Year IT Game Development · 14-Day Sprint Project

---

## 🎮 Play Now

👉 **[Play on GitHub Pages](https://yourusername.github.io/apex-dash)**

No installation. No downloads. Opens directly in your browser.

---

## 📸 Screenshots

| Menu | Gameplay | Finish Screen |
|------|----------|---------------|
| ![Menu](assets/screenshot-menu.png) | ![Gameplay](assets/screenshot-race.png) | ![Finish](assets/screenshot-finish.png) |

---

## 📖 Description

**Apex Dash** is a single-level time trial racing game where your goal is simple: reach the finish line as fast as possible.

The track is a technical circuit with tight corners, a fast straight, and a central island — every run rewards players who find the perfect racing line. Hit yellow speed boost pads to surge ahead, and avoid red obstacle barrels that cost you precious seconds. 

The signature feature is the **Ghost System**: your best run is recorded and replayed as a translucent blue car. You're always racing against yourself, shaving milliseconds off your personal best. Top 5 times are saved to a local leaderboard.

---

## 🕹️ Controls

| Key | Action |
|-----|--------|
| `W` / `↑` | Accelerate |
| `S` / `↓` | Brake / Reverse |
| `A` / `←` | Steer Left |
| `D` / `→` | Steer Right |
| `R` | Restart Race |
| `Space` / `Enter` | Start (from Menu / Finish screen) |

---

## ✨ Features

- **Ghost Replay System** — Your personal best is recorded frame-by-frame and replayed as a ghost car on subsequent runs. Stored in `localStorage` so it persists between sessions.
- **Speed Boost Pads** — Yellow ⚡ pads grant a temporary speed burst. Learn the track to optimise which ones to hit.
- **Obstacle Hazards** — Red ✕ barrels slow you down significantly on contact. Precision cornering is rewarded.
- **Millisecond Timer** — Live race timer with 3-decimal precision. Every millisecond counts.
- **Persistent Leaderboard** — Top 5 times saved locally. Your records survive browser refreshes.
- **Visual HUD** — Live speedometer bar, current time, best time, and boost/penalty flash effects.
- **Screen States** — Complete game loop: animated Menu → Race → Score/Finish screen with leaderboard.

---

## 🗂️ Project Structure

```
apex-dash/
├── index.html          ← Website landing page
├── team.html           ← Team information page
├── game/
│   └── index.html      ← Standalone game (HTML5 Canvas)
├── assets/
│   ├── screenshot-menu.png
│   ├── screenshot-race.png
│   └── screenshot-finish.png
└── README.md
```

---

## 🛠️ Tech Stack

| Technology | Usage |
|-----------|-------|
| HTML5 Canvas API | Game rendering (track, cars, HUD) |
| Vanilla JavaScript | Game loop, physics, collision detection |
| `localStorage` | Ghost data + leaderboard persistence |
| CSS3 | Website animations and layout |
| Google Fonts | Bebas Neue, DM Sans, Share Tech Mono |
| GitHub Pages | Deployment |

---

## 👥 Team

### [Your Name] — Lead Developer · Game Systems
- Vehicle physics and canvas rendering
- Ghost replay system and localStorage integration
- Timer, checkpoint, and finish line logic
- Speed boost and obstacle collision detection
- Menu and game-over screen implementation

🔗 [github.com/yourusername](https://github.com/yourusername)

---

### [Partner Name] — UI/UX Developer · Web & Level Design
- Track layout design and obstacle placement  
- HUD, leaderboard display, and score screens
- GitHub Pages website (landing page + team page)
- Visual theming, CSS animations, and asset creation
- README documentation and screenshots

🔗 [github.com/partnerusername](https://github.com/partnerusername)

---

## 🚀 Running Locally

```bash
git clone https://github.com/yourusername/apex-dash.git
cd apex-dash

# Option 1: Open directly (game works offline)
open index.html

# Option 2: Use a local server (recommended)
npx serve .
# Then visit http://localhost:3000
```

> **Note:** The game can be opened directly as a file (`file://`) since it uses no server-side code. However, a local server avoids any `iframe` origin restrictions when embedding the game in the website.

---

## 📋 Project Requirements Checklist

- [x] **Menu Screen** with title, controls reference, and start prompt
- [x] **Playable Level** with vehicle physics, track, boosts, obstacles
- [x] **Score/Finish Screen** with final time, leaderboard, and replay option
- [x] **Ghost System** — records and replays best run
- [x] **2-Page Website** — Landing page + Team page
- [x] **GitHub Pages** deployment
- [x] **5+ commits per student** (see commit history)
- [x] **README** with description, controls, and screenshots

---

## 📅 Development Sprint

| Days | Phase |
|------|-------|
| 1–2 | Repo setup, wireframes, role assignment |
| 3–7 | Core game loop, physics, track design, basic site |
| 8–11 | Ghost system, HUD polish, website integration |
| 12–13 | Bug fixes, cross-browser testing, README + screenshots |
| 14 | Final defence and walkthrough |

---

*© 2025 Binary Lap Studios — Built for 2nd Year IT Game Development*
