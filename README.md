# Memory Card Game

**Student:** Suhani | 2nd Year CSE-IOT III Sem | USN: 25BTRCO051

A card-matching game with three difficulty levels, a move counter, a timer and saved best scores.

## OVERVIEW
Memory Card Game shows a grid of face-down cards. The player flips two at a time to find matching emoji pairs. The game is won when every pair is matched, and the move count and time are compared with the saved best for that level.

## TECH STACK
- Frontend: HTML5, CSS3 (Grid, 3D flip with perspective and backface-visibility, transitions)
- Logic: vanilla JavaScript (Fisher-Yates shuffle, setInterval, event listeners)
- Storage: browser localStorage for best scores

## HOW IT WORKS
newGame() copies the emoji list into pairs, shuffles it and builds one card element per entry. Clicking a card flips it. The first flip starts the timer. On the second flip the moves count goes up and the two symbols are compared. A match locks both cards in green. A mismatch locks the board for 0.8 seconds and then flips both back. When all pairs are matched, the best score for that level is updated if beaten.

## KEY FEATURES
- Easy (12 cards), Medium (16 cards) and Hard (24 cards)
- Smooth 3D card flip
- Move counter and timer
- Best score saved for each level
- Board locking so fast clicking cannot break the game

## USES
Practising arrays, shuffling, timers and CSS animation, or a quick brain game.

## HOW TO RUN
Open index.html in any browser. No installation or internet connection is needed.
