# 🚀 Escape Galaxy



<p align="center">
  

https://github.com/user-attachments/assets/9f16132c-ae64-4a7a-bd49-f6a34704f863


</p>



<p align="center">
  <img src="https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black" alt="JavaScript">
  <img src="https://img.shields.io/badge/p5.js-ED225D?style=for-the-badge&logo=p5.js&logoColor=white" alt="p5.js">
  <img src="https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white" alt="HTML5">
  <img src="https://img.shields.io/badge/Canvas-2D-black?style=for-the-badge" alt="Canvas">
</p>

<p align="center">
  <strong>A 2D Vertical Space Shooter built with JavaScript, p5.js & p5.play.js</strong>
</p>

<p align="center">
  Fight through alien invasions, destroy hostile UFOs, survive deadly laser attacks,
  defeat the final boss, and make your escape back to Earth.
</p>

<p align="center">
  <a href="#-gameplay">Gameplay</a> •
  <a href="#-features">Features</a> •
  <a href="#-levels">Levels</a> •
  <a href="#-controls">Controls</a> •
  <a href="#-installation">Installation</a> •
  <a href="#-future-roadmap">Roadmap</a>
</p>

---

## 🌌 About The Game

**Escape Galaxy** is my first game development project, inspired by classic arcade-style space shooter games.

You take control of **AstroJet**, a spaceship travelling through hostile space. What begins as a simple alien assault quickly escalates into a full-scale UFO invasion and eventually a final battle against a powerful alien boss.

The goal is to survive, score enough points to progress through each stage, collect health boosts, upgrade your weapons, and ultimately defeat the boss to return safely to Earth.

> **Your ship is damaged. The galaxy is hostile. Earth is waiting.**

---

# 🎮 Gameplay

<p align="center">
  <img src="screenshots/gameplay.gif" alt="Escape Galaxy Gameplay" width="800">
</p>

> Replace `screenshots/gameplay.gif` with your actual gameplay GIF or video preview.

Escape Galaxy follows a progressive arcade-style gameplay loop:

```text
        🚀 START
           │
           ▼
   👽 ALIEN ASSAULT
           │
       500 POINTS
           │
           ▼
    🛸 UFO INVASION
           │
      1000 POINTS
           │
           ▼
      👾 BOSS BATTLE
           │
        20 HITS
           │
           ▼
       🌍 VICTORY
```

---

# ✨ Features

### 🚀 Player System

* Mouse-controlled spaceship
* Horizontal movement
* Projectile-based combat
* Three starting lives
* Health restoration through power-ups
* Multiple weapon upgrades

### 👽 Enemy System

* Falling alien enemies
* Meteor obstacles
* Hostile UFOs
* Enemy laser attacks
* Final alien boss
* Progressive difficulty

### 🔫 Combat System

* Fireball projectiles
* High-damage missiles
* Mystical trident projectiles
* Enemy laser patterns
* Boss triple-laser attacks

### 🌌 Game Systems

* Score tracking
* Level progression
* Health management
* Enemy spawning
* Collision detection
* Power-up spawning
* Multiple game states
* Victory and Game Over conditions

### 🔊 Audio

The game includes custom audio for:

* Background music
* Shooting
* Taking damage
* Health boosts
* Victory
* Game events

---

# 🌠 Levels

## Level 0 · Start Screen

The journey begins at the main menu.

Players can choose between:

**PLAY**

Start the mission.

**INFO**

View the game instructions and controls.

---

## Level 1 · Alien Assault

The first combat stage introduces the core mechanics.

### 👽 Falling Aliens

Aliens enter the screen from above.

**Reward: +100 points**

### ☄️ Meteors

Meteors fall through the battlefield and damage AstroJet on collision.

**Damage: -1 Life**

### ❤️ Health Boost

Health boosts periodically appear from the top of the screen.

**Reward: +1 Life**

### 🔥 Weapon

**Fireballs**

### 🎯 Objective

Reach:

**500 Points**

to unlock Level 2.

---

## Level 2 · Invasion of UFOs

The battlefield becomes significantly more dangerous.

### 🛸 UFOs

Advanced UFO enemies attack AstroJet while firing deadly vertical laser beams.

### 🚀 Weapon Upgrade

**Missiles**

Missiles replace the Fireballs and provide increased damage against UFO enemies.

### 🎯 Objective

Reach:

**1000 Points**

to unlock the final boss battle.

---

## Level 3 · Boss Battle

The final confrontation begins.

A massive alien boss appears at the top of the battlefield.

### 👾 Boss

**Health: 20 Hits**

The boss attacks using multiple laser patterns.

### ⚡ Attack Patterns

* 🔴 Red lasers
* 🔵 Blue lasers
* Triple-laser patterns
* Rapid-fire attacks

### 🔱 Final Weapon

**Mystical Trident**

### 🎯 Objective

Survive the laser barrage and land **20 successful hits** on the boss.

---

# 🌍 Victory

Defeating the boss triggers the final victory state.

The game transitions to an Earth-themed background and displays:

```text
████████████████████████

        YOU WON!

████████████████████████
```

The mission is complete.

---

# 💀 Game Over

AstroJet begins the mission with:

**3 Lives**

If all lives are lost, the game transitions to the Game Over state.

Players can select:

**RESTART**

and attempt the mission again.

---

# 🕹️ Controls

|          Input         | Action                     |
| :--------------------: | -------------------------- |
| 🖱️ **Mouse Movement** | Move AstroJet horizontally |
|        **SPACE**       | Fire current weapon        |
|   🖱️ **Mouse Click**  | Interact with menu buttons |

Simple controls. Increasingly complicated survival.

---

# ❤️ Health System

AstroJet starts each run with:

```text
❤️ ❤️ ❤️
3 Lives
```

Lives can be lost through:

* ☄️ Meteor collisions
* ⚡ Enemy laser attacks
* 👾 Boss attacks

Lives can be restored by collecting:

**Health Boosts**

---

# 🔫 Weapon Progression

The player's arsenal evolves throughout the game.

```text
┌──────────────────────────┐
│        LEVEL 1            │
│                           │
│       🔥 FIREBALLS        │
└────────────┬─────────────┘
             │
             ▼
┌──────────────────────────┐
│        LEVEL 2            │
│                           │
│        🚀 MISSILES        │
└────────────┬─────────────┘
             │
             ▼
┌──────────────────────────┐
│        LEVEL 3            │
│                           │
│    🔱 MYSTICAL TRIDENT    │
└──────────────────────────┘
```

---

# 🧩 Game Architecture

The game is organized around different game states representing the player's progression.

```text
LEVEL 0
  │
  ├── PLAY
  │
  ▼
LEVEL 1
  │
  ├── Score < 500 → Continue
  │
  └── Score ≥ 500
          │
          ▼
      LEVEL 2
          │
          ├── Score < 1000 → Continue
          │
          └── Score ≥ 1000
                  │
                  ▼
              LEVEL 3
                  │
                  ├── Boss Alive → Continue Battle
                  │
                  └── Boss Defeated
                          │
                          ▼
                      LEVEL 4
                       VICTORY
```

If:

```text
Lives = 0
    │
    ▼
LEVEL 5
GAME OVER
    │
    ▼
RESTART
```

---

# 🛠️ Tech Stack

<p align="center">

|    Technology    | Role                                 |
| :--------------: | ------------------------------------ |
|  **JavaScript**  | Core game logic                      |
|     **p5.js**    | Rendering, animation and interaction |
|  **p5.play.js**  | Sprites, collisions and game objects |
| **HTML5 Canvas** | Game rendering                       |
|     **HTML5**    | Game structure                       |
|      **CSS**     | Interface styling                    |

</p>

---

# 📂 Project Structure

```text
Escape-Galaxy/
│
├── index.html
├── sketch.js
├── style.css
│
├── assets/
│   ├── images/
│   │   ├── player/
│   │   ├── enemies/
│   │   ├── boss/
│   │   └── backgrounds/
│   │
│   ├── sounds/
│   │   ├── shooting/
│   │   ├── damage/
│   │   ├── victory/
│   │   └── background/
│   │
│   └── sprites/
│
├── screenshots/
│   ├── start-screen.png
│   ├── level-1.png
│   ├── level-2.png
│   ├── boss-battle.png
│   ├── victory.png
│   └── gameplay.gif
│
└── README.md
```

> Update this structure to match the actual repository before publishing.

---

# ▶️ Installation

## Prerequisites

You only need:

* A modern web browser
* Git
* VS Code or another code editor

---

## Clone the Repository

```bash
git clone https://github.com/codingyash9-bit/Escape-Galaxy.git
```

```bash
cd Escape-Galaxy
```

---

## Run the Game

### Option 1 · Open Directly

Open:

```text
index.html
```

in your browser.

### Option 2 · VS Code Live Server

For the best experience:

1. Open the project in VS Code.
2. Install the **Live Server** extension.
3. Right-click `index.html`.
4. Select **Open with Live Server**.
5. Start playing.

---

# 📸 Screenshots

## Start Screen

<img width="370" height="170" alt="start" src="https://github.com/user-attachments/assets/f706a282-c5e1-4d33-b2b3-8b4645d5ff0e" />

---

## Alien Assault

<img width="150" height="389" alt="alien" src="https://github.com/user-attachments/assets/69f6f796-52fd-46c0-9632-e51f1920998d" />


---

## UFO Invasion

<img width="323" height="156" alt="UFO" src="https://github.com/user-attachments/assets/7d83b165-43f1-49ef-bb04-fc8f454e561a" />


---

## Boss Battle

<img width="225" height="225" alt="boss" src="https://github.com/user-attachments/assets/1c284ea1-9a24-4d09-8fbe-2688aaf48e6c" />


---

# 🧠 What I Learned

**Escape Galaxy** was my first game development project and gave me hands-on experience with the fundamentals of browser-based game development.

Through this project, I learned and implemented:

* Game loops
* Rendering and animation
* Mouse and keyboard input
* Sprite-based game objects
* Collision detection
* Projectile systems
* Enemy spawning
* Health and life systems
* Score tracking
* Level progression
* Power-up mechanics
* Weapon systems
* Boss mechanics
* Audio integration
* Game state management

Most importantly, the project helped me move from simply writing code to thinking about how multiple systems interact to create a complete playable experience.

---

# 🚀 Future Roadmap

Potential improvements for future versions:

* [ ] Additional levels
* [ ] More alien enemy types
* [ ] Additional bosses
* [ ] More weapon types
* [ ] Advanced power-ups
* [ ] Explosion and particle effects
* [ ] High-score system
* [ ] Global leaderboard
* [ ] Multiple playable spaceships
* [ ] Keyboard controls
* [ ] Mobile support
* [ ] Persistent player progression
* [ ] Difficulty modes
* [ ] Improved animations
* [ ] More advanced boss attack patterns

---

# 📊 Game Progression

|    Stage    | Challenge              | Weapon       |        Objective |
| :---------: | ---------------------- | ------------ | ---------------: |
| **Level 0** | Start Screen           | —            |    Start Mission |
| **Level 1** | 👽 Aliens + ☄️ Meteors | 🔥 Fireballs |       500 Points |
| **Level 2** | 🛸 UFOs + Lasers       | 🚀 Missiles  |      1000 Points |
| **Level 3** | 👾 Alien Boss          | 🔱 Trident   |          20 Hits |
| **Level 4** | 🌍 Victory             | —            | Mission Complete |
| **Level 5** | Game Over              | —            |          Restart |

---

# ⭐ Project Highlights

**Escape Galaxy** represents my first step into game development and real-time interactive programming.

The project combines:

```text
JavaScript
    +
p5.js
    +
p5.play.js
    +
Game Logic
    +
Animation
    +
Audio
    +
Collision Detection
    +
Level Design
    =
ESCAPE GALAXY
```

---

# 👨‍🚀 Author

### Yash Mahadeshvar

**FE · Artificial Intelligence & Data Science**

GitHub: [@codingyash9-bit](https://github.com/codingyash9-bit)

---

# ⭐ Show Your Support

If you enjoyed **Escape Galaxy**, consider starring the repository.

Every ⭐ helps the project reach more people.

---

<p align="center">
  <strong>🚀 Prepare the ship.</strong>
  <br>
  <strong>🌌 Survive the galaxy.</strong>
  <br>
  <strong>👾 Defeat the boss.</strong>
  <br>
  <strong>🌍 Make it home.</strong>
</p>

<p align="center">
  <strong>ESCAPE GALAXY</strong>
</p>
