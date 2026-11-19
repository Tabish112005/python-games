<<<<<<< HEAD
# 🎮 Python Games Collection

A curated collection of 2D arcade, racing, multiplayer, board, and reflex games built with **Python** and **Pygame**. This repository showcases diverse game development concepts—ranging from vector physics and AI waypoint navigation to sprite animation, mask-based collision detection, and local 2-player multiplayer.

![Python](https://img.shields.io/badge/Python-3.8%2B-blue?logo=python&logoColor=white)
![Pygame](https://img.shields.io/badge/Library-Pygame-yellow?logo=python&logoColor=white)
![Platform](https://img.shields.io/badge/Platform-Windows%20%7C%20macOS%20%7C%20Linux-brightgreen)
![License](https://img.shields.io/badge/License-MIT-orange)

---

## 📑 Table of Contents

- [🎮 Games Overview](#-games-overview)
- [🕹️ Featured Games Deep Dive](#️-featured-games-deep-dive)
  - [1. Aim Trainer](#1--aim-trainer)
  - [2. Car Game (Traffic Dodge)](#2--car-game-traffic-dodge)
  - [3. Car Racing 2.0 (Circuit & AI)](#3--car-racing-20-circuit--ai)
  - [4. Checkers](#4--checkers)
  - [5. Galaxy Fighters (2-Player Duel)](#5--galaxy-fighters-2-player-duel)
  - [6. Space Invader](#6--space-invader)
  - [7. Space Dodge](#7--space-dodge)
  - [8. Street Fighter (Engine Prototype)](#8--street-fighter-engine-prototype)
  - [9. Platformer (Framework)](#9--platformer-framework)
- [📦 Installation & Getting Started](#-installation--getting-started)
- [🚀 How to Run the Games](#-how-to-run-the-games)
- [📂 Project Directory Structure](#-project-directory-structure)
- [🧠 Game Engineering Highlights](#-game-engineering-highlights)
- [📜 License](#-license)

---

## 🎮 Games Overview

| Game | Category | Mode | Key Controls | Status |
| :--- | :--- | :--- | :--- | :--- |
| **[Aim Trainer](#1--aim-trainer)** | Reflex / Arcade | Single Player | Mouse Click | ✅ Complete |
| **[Car Game](#2--car-game-traffic-dodge)** | Endless Traffic Dodging | Single Player | `W` `A` `S` `D` / `P` | ✅ Complete |
| **[Car Racing 2.0](#3--car-racing-20-circuit--ai)** | Circuit Racing vs. AI | Single Player (vs AI) | `W` `A` `S` `D` | ✅ Complete (10 Levels) |
| **[Checkers](#4--checkers)** | Strategy / Board Game | 2 Players (Local) | Mouse Click | ✅ Complete |
| **[Galaxy Fighters](#5--galaxy-fighters-2-player-duel)** | Space Dogfight | 2 Players (Local Split) | `WASD`+`L-Ctrl` vs. `Arrows`+`R-Ctrl` | ✅ Complete |
| **[Space Invader](#6--space-invader)** | Retro Wave Shooter | Single Player | `W` `A` `S` `D` + `Space` | ✅ Complete |
| **[Space Dodge](#7--space-dodge)** | Reflex Survival | Single Player | `A` `D` | ✅ Complete |
| **[Street Fighter](#8--street-fighter-engine-prototype)** | 2D Fighting Platformer | 2 Players (Local) | `Arrows` + `A` `D` | 🚧 In Development |
| **[Platformer](#9--platformer-framework)** | Tile-based Platformer | Single Player | `A` `D` | 🚧 Engine Foundation |
| **Shooter** | Side-scroller Shooter | Single Player | - | 🚧 Prototype |
| **Quiz Game** | Terminal Trivia Quiz | Single Player | Keyboard / CLI input | 🚧 Starter |

---

## 🕹️ Featured Games Deep Dive

### 1. 🎯 Aim Trainer
A reaction-time and accuracy testing game. Targets dynamically spawn, expand, and shrink across the canvas. Click them before they vanish!

- **Folder:** `Aim Trainer/`
- **Main Script:** `main.py`
- **Features:**
  - Real-time performance statistics: elapsed time, target hit speed (targets/sec), hits counter, and lives.
  - End-game performance breakdown with accuracy percentage calculation.
- **Controls:**
  - `Left Mouse Click` : Click targets

---

### 2. 🏎️ Car Game (Traffic Dodge)
An arcade road challenge where the player maneuvers through heavy oncoming traffic on a multi-lane highway.

- **Folder:** `Car Game/`
- **Main Script:** `car_game.py`
- **Features:**
  - Main menu UI with interactive buttons and countdown screen.
  - On-screen instructions and pause/resume overlay.
  - Multi-car textures and collision response.
- **Controls:**
  - `W` : Accelerate
  - `S` : Brake
  - `A` / `D` : Steer Left / Right
  - `P` : Pause Game

---

### 3. 🏁 Car Racing 2.0 (Circuit & AI)
A top-down motorsport simulation featuring realistic vehicular physics and an intelligent computer opponent.

- **Folder:** `Car Racing 2.0/`
- **Main Script:** `main.py`
- **Features:**
  - **Physics Simulation:** Angular rotation, inertia, forward acceleration, reverse gear, and natural deceleration friction.
  - **Mask Collision:** Pixel-perfect mask checks bouncing cars off track walls.
  - **AI Waypoint Navigation:** The AI follows calculated tangent vectors along track waypoints, automatically scaling its top speed across 10 progressive difficulty levels.
  - **Telemetry HUD:** Real-time speedometer (`px/s`), level indicator, and lap stopwatch.
- **Controls:**
  - `W` : Forward Acceleration
  - `S` : Reverse / Decelerate
  - `A` / `D` : Steer Left / Right

---

### 4. 🏁 Checkers
A complete digital recreation of the classic board game with visual movement guidance and rule validation.

- **Folder:** `Checkers/`
- **Main Script:** `main.py`
- **Features:**
  - Automatic calculation and blue-dot indicators for all legal moves.
  - Diagonal jump and capture mechanics (including multi-piece skipping).
  - King piece promotion with crown rendering upon reaching the opposing board edge.
  - Alternating turn management and winner detection.
- **Controls:**
  - `Left Mouse Click` : Select piece & click highlighted destination square

---

### 5. 🚀 Galaxy Fighters (2-Player Duel)
A fast-paced local couch multiplayer space duel. Two spaceships face off across a central boundary barrier.

- **Folder:** `Galaxy Fighters/`
- **Main Script:** `main.py`
- **Features:**
  - Split battle zone separated by a central perimeter boundary.
  - Maximum bullet ammo cap on-screen to discourage blind spamming.
  - Dynamic audio for laser fire and grenade impact hits.
  - Visual health status bars and victory announcement screen.
- **Controls:**
  - **Player 1 (Yellow Ship - Left):**
    - `W` `A` `S` `D` : Move Up / Left / Down / Right
    - `Left Ctrl` : Fire Lasers
  - **Player 2 (Red Ship - Right):**
    - `Up` `Down` `Left` `Right` : Move
    - `Right Ctrl` : Fire Lasers

---

### 6. 👾 Space Invader
A retro vertical shooter inspired by arcade classics. Defend your quadrant against descending waves of hostile alien invaders.

- **Folder:** `Space Invader/`
- **Main Script:** `main.py`
- **Features:**
  - Procedural wave generation with progressive enemy swarm sizes.
  - Diverse enemy variants (Red, Green, Blue) each with distinct laser capabilities and random firing timers.
  - Player health bar and life tracking system.
  - Pixel-perfect mask collision handling for ships and lasers.
- **Controls:**
  - `W` `A` `S` `D` : Move ship in 4 directions
  - `Spacebar` : Shoot Lasers
  - `Mouse Click` : Start game from title screen

---

### 7. ☄️ Space Dodge
A survival test against a constant meteor shower in deep space.

- **Folder:** `space Dodge/`
- **Main Script:** `main.py`
- **Features:**
  - Dynamic scaling difficulty: star generation intervals shorten continuously as survival time increases.
  - Clean survival timer and instant collision detection.
- **Controls:**
  - `A` : Move Left
  - `D` : Move Right

---

### 8. 🥊 Street Fighter (Engine Prototype)
A 2D fighting platformer base containing sprite sheet assets, physics, and combat hitbox mechanics.

- **Folder:** `Street fighter/`
- **Main Script:** `main.py`
- **Features:**
  - Gravity simulation, jumping arc, and ground collision clamping.
  - Hitbox generation for horizontal attack ranges.
  - Rich asset pack included: animated warrior and wizard spritesheets, custom sound effects (`sword.wav`, `magic.wav`), and arcade fonts.
- **Controls:**
  - `Left` / `Right` : Move fighter
  - `Up` : Jump
  - `A` / `D` : Attack variations

---

### 9. 🏃 Platformer (Framework)
A 2D platforming foundation utilizing tiled background rendering and modular character sprite classes.

- **Folder:** `Platformer/`
- **Main Script:** `main.py`
- **Assets:** Extensive `Pixel Adventure` assets containing terrain tiles, fruit collectibles, animated traps (saws, spikes, trampolines), and enemy sprites.
- **Controls:**
  - `A` / `D` : Move Left / Right

---

## 📦 Installation & Getting Started

### Prerequisites
- **Python 3.8 or higher** installed on your machine.
- `pip` (Python package installer).

### 1. Clone the Repository
```bash
git clone https://github.com/your-username/your-repository-name.git
cd your-repository-name
```

### 2. Create a Virtual Environment (Recommended)
```bash
# Windows
python -m venv venv
.\venv\Scripts\activate

# macOS / Linux
python3 -m venv venv
source venv/bin/activate
```

### 3. Install Required Dependencies
All games run on **Pygame**:
```bash
pip install pygame
```
*(Or install via `pip install -r requirements.txt` if provided).*

---

## 🚀 How to Run the Games

> [!IMPORTANT]
> Because these games load assets (sprites, images, audio, and fonts) using relative paths, **always change directory (`cd`) into the specific game's folder before executing the script**.

Run any game from your terminal or command prompt:

```bash
# 🎯 Aim Trainer
cd "Aim Trainer"
python main.py

# 🏎️ Car Game (Traffic Dodge)
cd "../Car Game"
python car_game.py

# 🏁 Car Racing 2.0 (Circuit & AI)
cd "../Car Racing 2.0"
python main.py

# 🏁 Checkers
cd "../Checkers"
python main.py

# 🚀 Galaxy Fighters (2-Player Duel)
cd "../Galaxy Fighters"
python main.py

# 👾 Space Invader
cd "../Space Invader"
python main.py

# ☄️ Space Dodge
cd "../space Dodge"
python main.py

# 🥊 Street Fighter
cd "../Street fighter"
python main.py

# 🏃 Platformer
cd "../Platformer"
python main.py
```

---

## 📂 Project Directory Structure

```text
.
├── Aim Trainer/
│   └── main.py
├── Car Game/
│   ├── car_game.py
│   └── *.jpg (car models, tracks, menus)
├── Car Racing 2.0/
│   ├── main.py
│   ├── utils.py
│   └── imgs/ (cars, track borders, finish line)
├── Checkers/
│   ├── main.py
│   ├── assets/ (crown.png)
│   └── checkers/ (board.py, game.py, piece.py, constants.py)
├── Galaxy Fighters/
│   ├── main.py
│   └── Assets/ (spaceships, backgrounds, sound effects)
├── Platformer/
│   ├── main.py
│   └── assets/ (Pixel Adventure terrain, traps, items, characters)
├── Quiz Game/
│   └── quize_game.py
├── shooter/
│   └── main.py
├── space Dodge/
│   ├── main.py
│   └── bg.jpg
├── Space Invader/
│   ├── main.py
│   └── assets/ (pixel ships, lasers, background)
├── Street fighter/
│   ├── main.py
│   ├── fighter.py
│   └── assets/ (warrior & wizard sprites, audio, fonts)
└── README.md
```

---

## 🧠 Game Engineering Highlights

- **Vector Mathematics & Angles:** Trigonometric rotation (`math.atan`, `math.degrees`, `math.cos`, `math.sin`) to accurately position and orient moving objects in `Car Racing 2.0`.
- **Mask Collisions (`pygame.mask`):** Sub-pixel precision collision detection that ignores transparent sprite borders.
- **Finite State & Turn Handling:** Encapsulated turn logic and multi-step validation in `Checkers`.
- **Dynamic Difficulty Curves:** Algorithmic spawn rates that escalate challenge based on player survival time in `Space Dodge` and level loops in `Space Invader`.
- **Local Split-Keyboard Multiplayer:** Simultaneous multi-key registration via `pygame.key.get_pressed()` for fluid 2-player action without input locking.

---

## 🤝 Contributing

Contributions, feature additions, and bug fixes are welcome!
1. Fork the Project.
2. Create your Feature Branch (`git checkout -b feature/CoolGameFeature`).
3. Commit your Changes (`git commit -m "Add new powerup to Space Invader"`).
4. Push to the Branch (`git push origin feature/CoolGameFeature`).
5. Open a Pull Request.

---

## 📜 License

This project is open-source and available under the [MIT License](LICENSE).
Feel free to use the code for learning, educational purposes, and building your own games!
=======
# python-games
Python Games
>>>>>>> 8509e7eabb5fd4fd88d144fbc8f8ef6a29074a30
