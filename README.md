# 404: ERROR HEART NOT FOUND 

### `a Custom valentine’s multi-level puzzle game ♡`

**404: ERROR HEART NOT FOUND** is a browser-based puzzle game created as a Valentine's Day project for Cody.

Player progress' through five levels of riddles, grid-based mazes, collectibles, keys, locked paths, and level objectives in an interactive terminal-inspired environment.

This was my **first larger-scale programming project** — to fully disclose this is not perfect by any means but my first time combining multiple aspects, the game(s) were essentially broken a million times throughout their creation lol but finally came together in the end!

---

## ✦ Overview

The project combines a terminal inspired interface with a series of progressively structured maze puzzles.

The core gameplay loop is:

```
┌─────────────────────────────┐
│         SOLVE RIDDLE        │
└──────────────┬──────────────┘
               ↓
┌─────────────────────────────┐
│        ENTER THE MAZE       │
└──────────────┬──────────────┘
               ↓
┌─────────────────────────────┐
│       COLLECT FRAGMENTS     │
└──────────────┬──────────────┘
               ↓
┌─────────────────────────────┐
│     UNLOCK THE OBJECTIVE    │
└──────────────┬──────────────┘
               ↓
┌─────────────────────────────┐
│        COMPLETE LEVEL       │
└──────────────┬──────────────┘
               ↓
              ♡
```

Each level introduces a maze, puzzle elements, and a progression objective before unlocking the next stage.

---

## ✦ Features

* ♡ Five playable maze levels
* ✦ Grid-based player movement
* ✦ Keyboard controls
* ✦ Level-specific riddles
* ✦ Collectible fragments
* ✦ Keys and locked pathways
* ✦ Dynamic objective spawning
* ✦ Level completion states
* ✦ Progressive level unlocking
* ✦ Terminal-inspired interface
* ✦ CSS animations and visual effects
* ✦ Sound effects
* ✦ Introductory and ending sequences
* ✦ HTML Canvas-based maze rendering
* ✦ Client-side game state management

---

## 🎮 Gameplay

### Movement

Players navigate each maze using the arrow keys.

| Key | Action     |
| :-: | ---------- |
| `↑` | Move up    |
| `↓` | Move down  |
| `←` | Move left  |
| `→` | Move right |

### Collectibles

Each level contains collectible fragments distributed throughout the maze.

Collecting the required fragments allows the level's primary objective to become available.

### 🔑 Keys & Locked Paths

Later levels introduce keys and locked barriers.

Players must locate the appropriate key before accessing certain areas of the maze, adding an additional exploration and progression mechanic.

### Level Progression

```
Riddle
  ↓
Maze
  ↓
Collect Fragments
  ↓
Unlock Objective
  ↓
Recover Objective
  ↓
Complete Level
  ↓
Next Level
```

The final level concludes with the system restoration sequence.

---

## ✦ Technical Implementation

### HTML

HTML provides the structure for the game's:

* Interface
* Game screens
* Buttons
* Riddle displays
* Dialogue
* Canvas
* Level completion screens

### CSS

CSS handles the visual design and presentation, including:

* Terminal-inspired styling
* Typography
* Layout
* Buttons and interactive elements
* Borders
* Animations
* Transitions
* Glitch effects
* Color and visual hierarchy

### JavaScript

JavaScript manages the game's core functionality and state.

The application uses JavaScript for:

* Player movement
* Keyboard event handling
* Maze logic
* Collision detection
* Collectible tracking
* Key collection
* Locked-path logic
* Objective spawning
* Riddle progression
* Screen transitions
* Level progression
* Audio interaction
* Game completion

### HTML Canvas

The maze environments are rendered using the HTML Canvas API.

Each maze is represented as a grid containing different tile types:

```
0 → Open space
1 → Wall
2 → Collectible
3 → Locked barrier
4 → Key
5 → Objective
```

This structure allows the movement and collision systems to be reused across multiple levels while changing the maze layout.

---

## ✦ Project Structure

```text
404-ERROR-HEART-NOT-FOUND/
│
├── index.html
├── README.md
│
└── assets/
    └── bunny-hack/
        ├── bunny.png
        └── evil-laugh.wav
```

The current version intentionally keeps the project lightweight, with the primary application logic contained within `index.html` and external media stored in the `assets` directory.

---

## ✦ Development

This project was my first **"big project."**

Before building this, most of my programming practice consisted of smaller exercises, experiments, and individual features. This was the first time I had to think about how multiple systems could work together inside one complete application.

Rather than building one isolated feature at a time, I had to manage an entire game loop and its different states.

Some of the systems I built included:

```
┌──────────────────────┐
│     User Interface   │
├──────────────────────┤
│      Game State      │
├──────────────────────┤
│    Movement System   │
├──────────────────────┤
│      Maze System     │
├──────────────────────┤
│   Collectible Logic  │
├──────────────────────┤
│    Key / Door Logic  │
├──────────────────────┤
│   Puzzle Progression │
├──────────────────────┤
│   Level Completion   │
└──────────────────────┘
```

Building these systems together gave me my first experience with the additional planning and debugging that comes with a larger interactive project.

---

## ✦ What I Learned

This project helped me build a stronger understanding of both JavaScript and the development process as a whole.

### JavaScript

* Functions and reusable logic
* Arrays and nested arrays
* Conditional logic
* Event listeners
* Keyboard input
* DOM manipulation
* State management
* Collision detection
* Game progression

### HTML & CSS

* Structuring interactive interfaces
* Managing multiple application states
* Styling interactive elements
* Creating animations and transitions
* Building a consistent visual system

### Canvas

* Rendering grid-based environments
* Working with coordinates
* Drawing game elements
* Updating the game based on player movement

### Development

* Breaking a larger idea into smaller features
* Debugging unexpected behavior
* Testing changes incrementally
* Organizing assets
* Using Git and GitHub
* Iterating on an existing implementation
* Completing a project from concept to finished product

---

## ✦ Challenges

One of the biggest challenges was coordinating multiple interactive systems within the same application. And to be honest the incorporation of assets (or lack thereof) and the music/media files. I ended up trying to do everything with custom code pixel animation- this project would’ve been much easier if I had incorporated the assets correctly! 

As new mechanics were introduced, systems such as movement, collectibles, keys, locked paths, level progression, and screen transitions all needed to interact with the game's current state.

This required learning to think more carefully about:

* When the game should accept player input
* Which conditions should allow movement
* How collected items should change the environment
* When objectives should become available
* How level completion should trigger progression
* How to prevent interactions from occurring during the wrong game state

Working through these problems was one of the most valuable parts of building the project.

---

## ✦ Design

The visual direction combines a **terminal / corrupted-system aesthetic** with a Valentine's theme.

The interface uses:

* Dark backgrounds
* Monospace typography
* Green terminal-style elements
* Pink accents
* Pixel-inspired graphics
* Glitch effects
* Minimal interface components

The intention was to make the game feel like an interactive system that gradually reveals its actual purpose as the player progresses.

---

## ♡ Why I Made It

I wanted to make something that could be an interactive gift for Valentine’s day!

Although the project was personal, it also gave me an opportunity to challenge myself with something significantly larger than the projects I had built previously.

---


## ✦ Future Improvements

If I continue developing the project, possible improvements include:

* Refactoring JavaScript into separate modules
* Separating HTML, CSS, and JavaScript into dedicated files
* Improving code organization and maintainability
* Adding additional levels
* Expanding the puzzle mechanics
* Adding more audio and visual effects
* Implementing persistent game progress
* Adding mobile or touch controls
* Improving accessibility and keyboard navigation
* Adding a dedicated restart / reset system

---

## ✦ Status

**Completed ♡**

The current version includes five playable levels, puzzle progression, collectible and key mechanics, locked paths, level objectives, audio, visual effects, and the final ending sequence.
