# Trex_game

A lightweight, browser-based endless runner inspired by Chrome’s Dino game. Built with **JavaScript**, **p5.js**, and **p5.play**, it features sprite animation, procedural obstacles, collision detection, scoring, and a clean restart flow—all on the HTML5 canvas.

---

## Features

* **Smooth gameplay loop** with PLAY/END states and instant restart
* **Procedural spawning** of obstacles and clouds (parallax look)
* **Sprite animations & hitboxes** via p5.play groups
* **Dynamic difficulty** as score increases (optional)
* **On-screen HUD**: score, game over & restart UI

## Controls

* **Jump:** `Space` or `↑`
* **(Optional) Duck:** `↓`
* **Restart:** Click/Tap **Restart** or press `Space` after game over

## Tech Stack

* **Language:** JavaScript
* **Libraries:** \[p5.js], \[p5.play]
* **Rendering:** HTML5 Canvas

## Getting Started

### 1) Download

Extract the project (e.g., `Trex_game-master/`).

### 2) Run a local server (recommended)

Most browsers block local file access; a tiny server avoids CORS issues.

**Option A — Python (built-in):**

```bash
cd Trex_game-master
python3 -m http.server 8000
# open http://localhost:8000 in your browser
```

**Option B — VS Code Live Server:**

* Open the folder in VS Code
* Install the *Live Server* extension
* Right-click `index.html` → **Open with Live Server**

### 3) Play

Open your browser at `http://localhost:8000` (or the Live Server URL), then press **Space** to start.

## Project Structure (typical)

```
Trex_game-master/
├─ index.html          # loads p5.js, p5.play, and your sketch
├─ sketch.js           # main game loop & state management
├─ sprites/            # trex, obstacles, clouds, ground, UI
├─ assets/             # sounds, fonts (optional)
└─ styles.css          # minimal styling (optional)
```

> Your actual filenames may differ—adjust as needed.

## Configuration (common tweaks)

Open your main JS file (e.g., `sketch.js`) and look for constants/variables such as:

* **Spawn rates** for obstacles/clouds
* **Gravity / jump velocity**
* **Speed scaling** with score
* **Hitbox sizes** (colliders)
* **Sprite image paths**

Tune these to change difficulty and feel.

## Troubleshooting

* **Blank page / errors:** Check the browser console (F12 → Console).
* **Assets not found:** Verify file paths and case sensitivity.
* **No jump / no input:** Ensure the canvas has focus (click it once).
* **Nothing loads from file system:** Serve via a local server (see above).

## Roadmap (nice-to-have)

* Mobile touch controls & pause menu
* Power-ups (shield, double jump, slow-mo)
* High-score persistence (localStorage)
* Day/night cycle & more obstacle types
* Sound effects & music toggle

## Credits

* Inspired by the **Chrome Dino** offline game
* Built with **p5.js** and **p5.play**
  
---

**Enjoy the run!**
