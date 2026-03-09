# Pig Game

A two-player browser dice game built with vanilla JavaScript, styled with a cyberpunk hi-tech aesthetic.

---

## Gameplay

Two players take turns rolling a dice. The goal is to be the first to reach **100 points**.

### Rules

- **Roll** — throw the dice. The result adds to your *current score*
- If you roll a **1** — your current score is lost and the turn passes to the opponent
- **Hold** — bank your current score to your total and pass the turn
- First player to reach **100 points wins**
- **New Game** — resets everything and starts fresh

---

## Features

- Two-player local multiplayer
- Animated cyberpunk UI — scan beam, neon glow, floating dice, flicker effects
- Fully responsive — desktop, tablet, mobile
- Zero dependencies (no frameworks, no libraries)
- Fast dev/build via Vite

---

## Tech Stack

| Layer | Tool |
|---|---|
| Logic | Vanilla JavaScript (ES Modules) |
| Markup | HTML5 |
| Styles | CSS3 (Grid, custom properties, keyframe animations) |
| Font | [Orbitron](https://fonts.google.com/specimen/Orbitron) via Google Fonts |
| Build | [Vite](https://vite.dev/) |

---

## Getting Started

### Prerequisites

- [Node.js](https://nodejs.org/) v18+

### Install & run

```bash
# clone or download the repo, then:
cd game2

npm install
npm run dev
```

Open `http://localhost:5173` in your browser.

### Build for production

```bash
npm run build
# output → dist/
```

### Preview production build

```bash
npm run preview
```

---

## Project Structure

```
game2/
├── public/
│   └── dice_png/          # Dice face images (dice-1.png … dice-6.png)
├── src/
│   ├── main.js            # All game logic (~95 lines, no frameworks)
│   └── style.css          # Cyberpunk UI + responsive layout
├── index.html             # App shell
├── package.json
└── README.md
```

---

## Responsive Breakpoints

| Viewport | Layout |
|---|---|
| **Desktop** `> 860px` | 3-column grid — Player / Controls / Player |
| **Tablet** `560–860px` | Same grid, scaled fonts and spacing |
| **Mobile** `< 560px` | Vertical stack — Player 1 → Controls row → Player 2 |

---

## License

MIT — do whatever you want with it.
