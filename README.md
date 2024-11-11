```markdown
# Spooky Match Game

This project is a spooky-themed memory matching game built using HTML, CSS, and JavaScript.  The goal is to find all the matching pairs of spooky images before the timer runs out.


## Functionality

The game starts with a welcome screen (`index.html`) featuring a spooky animated title and a "Let's Play" button. Clicking this button takes the player to the game screen (`index1.html`).

On the game screen, cards are laid out face down. The player flips two cards at a time. If the cards match, they remain face up. If they don't match, they flip back over. The player wins when all cards are matched before the timer reaches zero.  If the timer runs out, the game is over.  The player can restart the game at any time by clicking the overlay message that appears.

### Game Logic

* **Card Flipping:** Clicking on a card flips it to reveal its image.
* **Matching Logic:** The game checks if the two flipped cards match.
* **Win Condition:**  The game is won when all pairs are matched.
* **Lose Condition:** The game is lost when the timer reaches zero.
* **Timer:** A timer counts down, adding a challenge to the game.
* **Flip Counter:** A counter keeps track of the number of card flips made by the player.
* **Audio Feedback:** Sound effects enhance the game experience (flipping, matching, victory, game over, and background music).
* **Restart Functionality:** Clicking the game over or victory message restarts the game.

## Technologies Used

### HTML (index.html, index1.html)

*   **Semantic HTML:** Uses elements like `<header>`, `<section>`, `<div>`, `<span>`, `<img>`, etc. to structure content logically.
*   **Links:** `<a>` tag used for navigation between the start screen and the game screen.
*   **Meta Tags:** Used for viewport settings and character set definition.

### CSS (style.css, style1.css)

*   **Custom Fonts:** Uses external fonts for stylized text.
*   **Animations:**  CSS animations are used for the burning text effect on the start screen and the dancing card effect on match.
*   **Background Images:** Sets background images for both start and game screens.
*   **Flexbox:**  Used for layout and alignment on the start screen.
*   **Grid:** Used to create the card layout on the game screen.
*   **Transforms:** Used for card flipping and hover effects.
*   **Transitions:** Smooths out animations and transitions.
*   **Media Queries:** Makes the game responsive to different screen sizes.
*   **Custom Cursors:** Implements custom mouse cursors for a spooky theme.

### JavaScript (script.js)

*   **Classes:** Uses classes `AudioController` and `MixOrMatch` to organize code and manage game logic.
*   **DOM Manipulation:** Selects and manipulates HTML elements to update game state and display information.
*   **Event Listeners:**  Listens for click events on cards and overlay messages to handle user interaction.
*   **Timer:** Implements a timer using `setInterval`.
*   **Audio Control:**  Plays and controls sound effects using the `Audio` object.
*   **Game Logic:** Implements the core game mechanics such as shuffling cards, checking for matches, handling win/loss conditions, and restarting the game.
*   **Fisher-Yates Shuffle Algorithm:** Ensures random card arrangement for each game.


## How to Play

1. Open `index.html` in your web browser.
2. Click the "Let's Play" button to start the game.
3. Click on cards to flip them over and find matching pairs.
4. Match all pairs before the timer runs out to win!


## Future Improvements

*   Implement a scoring system.
*   Add different difficulty levels.
*   Include more card variations.
*   Improve accessibility.
```