# Drum Kit Web App

This is an interactive Drum Kit web application built using HTML, CSS, and JavaScript. The app allows users to play drum sounds by pressing specific keys on the keyboard or by clicking the on-screen drum buttons. Each key corresponds to a different drum sound, and visual feedback is provided with a CSS animation when a key is pressed.

## Features

- **Interactive Drum Sounds**: Each key on the keyboard corresponds to a different drum sound (e.g., Clap, HiHat, Kick, etc.).
- **Visual Feedback**: When a key is pressed, the corresponding key on the screen animates, showing the user which key has been pressed.
- **Keyboard and Mouse Input**: Users can play the sounds either by pressing the appropriate keys on their keyboard or by clicking on the on-screen buttons.

## How It Works

### HTML
- The HTML structure includes `div` elements with `data-key` attributes that map to different sounds and the keys they correspond to.
- Each sound is associated with an `<audio>` element, where the `data-key` attribute matches the keyboard key.

### JavaScript
- The `keydown` event listener is used to detect when a user presses a key on the keyboard. The keycode is used to select the correct `<audio>` element and play the corresponding sound.
- When a key is pressed, the `.playing` class is added to the corresponding `.key` element to trigger a visual animation using CSS.
- The transition end event is used to remove the `.playing` class after the animation completes.

### CSS
- The `.playing` class triggers a CSS animation on the pressed key, making it "pop" with a transform effect.
  
## Setup Instructions

1. **Clone the repository** or download the files.
2. Open the `index.html` file in your web browser.
3. Press any of the designated keys on your keyboard (A, S, D, F, G, H, J, K, L) to play the corresponding drum sounds.
4. Alternatively, click on the drum buttons on the screen to play the sounds.

## File Structure

```plaintext
├── index.html        # The main HTML file containing the structure of the drum kit
├── style.css         # The CSS file that styles the drum kit and key animations
└── script.js         # The JavaScript file that controls the functionality of the app
