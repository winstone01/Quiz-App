# Quiz App — Vol 1.3

A lightweight, responsive **Quiz App** built with vanilla HTML, CSS, and JavaScript.  
Includes a start screen, timed multiple-choice questions, instant answer feedback, and a final score summary with restart.

---

## Features

- **Start screen** to begin the quiz
- **Countdown timer** per question (auto-advances when time runs out)
- **Randomised questions and options** on each run
- **Instant feedback** (correct / incorrect styling)
- **Score summary** at the end
- **Restart** button to play again

---

## Built With

- **HTML5**
- **CSS3**
- **JavaScript (ES6)**
- **Font Awesome** (icons)
- **Google Fonts** (Oswald)

---

## Getting Started

### Run locally
1. Download / clone this repository
2. Open `index.html` in your browser  
   *(Optional: use VS Code Live Server for auto-reload.)*

---

## How It Works (Logic Overview)

- Questions are stored in a `quizArray` object (question, options, correct answer).
- On start:
  - Questions are **shuffled**
  - Options are **shuffled**
  - Question cards are generated dynamically and displayed one at a time
- The timer counts down per question:
  - When it hits 0, it automatically moves to the next question
- Clicking an option:
  - Highlights correct/incorrect choices
  - Increments score if correct
  - Disables options after selection
- At the end:
  - The app displays a final **score screen**
  - Restart resets state and runs again

---

## Project Structure

/
├─ index.html  
├─ style.css  
└─ script.js  

---

## Improvements for Next Version

- [ ] Fix disabled option text color (currently set to transparent)
- [ ] Stop timer immediately after selecting an answer (also for correct answers)
- [ ] Prevent multi-click scoring (lock a question after first selection)
- [ ] Add question categories / difficulty
- [ ] Add progress bar + better accessibility (focus states, ARIA labels)
- [ ] Store high score with localStorage

---

## Author

**Winstone Anderson**  
UI-focused frontend developer building clean, responsive web interfaces.

---

## License

MIT 
