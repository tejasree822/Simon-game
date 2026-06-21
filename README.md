# Simon Game 🎮

A browser-based memory game inspired by the classic Simon Game. The objective is to remember and repeat an increasingly long sequence of colors and sounds.

---

## How to Play

1. Press any key to start the game.
2. Watch the button that flashes.
3. Click the button shown by the game.
4. A new color is added to the sequence every level.
5. Repeat the entire sequence in the correct order.
6. The game ends if you click the wrong button.
7. Press any key to restart and try again.

---

## Features

- Random sequence generation
- Sound effects for each color
- Button press animations
- Level tracking
- Game over detection
- Restart functionality

---

## Technologies Used

- HTML5
- CSS3
- JavaScript
- jQuery

---

## Project Structure

```text
Simon-Game/
│
├── index.html
├── styles.css
├── game.js
│
└── sounds/
    ├── red.mp3
    ├── blue.mp3
    ├── green.mp3
    ├── yellow.mp3
    └── wrong.mp3
```

---

## Game Logic

### 1. Start the Game

- The game waits for the first key press.
- A `started` flag ensures the game starts only once.
- The first call to `nextSequence()` begins the game.

### 2. Generate a Random Sequence

- A random color is selected from:
  - Red
  - Blue
  - Green
  - Yellow
- The selected color is added to the `gamePattern` array.
- The corresponding button flashes and plays its sound.

### 3. User Input

- Each button click is stored in the `userClickedPattern` array.
- The clicked button plays its sound and shows a press animation.

### 4. Check the Answer

- After every click, the latest user input is compared with the corresponding color in the game pattern.
- If the input is correct, the game continues.
- If the entire sequence is completed correctly, the next level begins.

### 5. Game Over

- A wrong sound is played.
- A game-over animation is displayed.
- The title changes to indicate the game has ended.
- The game variables are reset for a restart.

---

## Future Improvements

- High score tracking
- Mobile-friendly design
- Difficulty levels
- Local storage support
- Dark mode

---

## Author

**Sai Teja Sree**

B.Tech in Mathematics and Computing, NIT Warangal

---
