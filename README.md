# Memory Match Game

A simple memory match game built with React + TypeScript.
The player’s goal is to find all matching pairs before time runs out or all lives are lost.

## 🛠️ Tech Stack

- **Vite + React + TypeScript**
- **Zustand** 
- **Framer Motion**
- **MUI**
- **FSD (Feature-Sliced Design)**

## 🎮 Game Rules

- The board is a **6x6 grid**.
- There are **18 pairs** of matching cards (36 cards total).
- All cards are briefly revealed before the game starts.
- After that, the cards are hidden and the game begins.

### Gameplay:

1. The player clicks on two cards.
2. If the cards match:
   - They stay open.
   - The player earns points.
3. If the cards do not match:
   - They are hidden again after a short delay.
   - The player loses one life.
   - All remaining closed cards **shuffle positions**.
4. The player has **3 lives**.
5. The game ends when:
   - All pairs are found (win),
   - Time runs out, or
   - All lives are lost (lose).

### Scoring:

- Points are awarded for each correct match.
- Bonus points are given for consecutive matches and remaining time.
- At the end, the player can enter a name and save their score to the local leaderboard.

## 🚀 Getting Started

```bash
git clone https://github.com/yourusername/memory-match-react.git
cd memory-match-react
npm install
npm run dev
