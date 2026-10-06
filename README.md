# Snake 3D

**The classic snake game, rebuilt in 3D and playable in any browser.**

Snake 3D is a single-file web game. You steer a glowing snake around a floating 3D board, eat fruit to grow, and try to beat your best score. It runs with no build step and no server, so you can play it by opening one file.

![Snake 3D screenshot](/pic/znake.png)



## Key features

- Real 3D graphics with soft shadows, glowing walls and a smoothly gliding snake
- Animated gradient background that drifts through blue, violet and magenta, speeds up as the game gets faster, pulses when you eat and turns red when you crash
- Polished HUD with score, best, length, a level meter, floating score pop-ups and level-up banners
- Start, pause and game-over cards with key hints and an end-of-game stats summary
- Camera that orbits on the menu and follows the action during play
- Two camera views: angled and top-down (toggle with the button in the top right)
- Particle effects and short sound effects when you eat or crash
- Game speeds up as you eat more fruit
- Best score saved in your browser
- Pause with `P` or `Esc`, and automatic pause when you switch tabs
- Keyboard, touch swipe and on-screen d-pad controls, so it works on desktop and mobile
- Adaptive layout: desktop gets a keyboard shortcut legend, phones get a d-pad and swipe controls, and portrait and landscape both fit the board between the top bar and the controls

## Install and run (about 5 minutes)

You need a modern browser (Chrome, Edge, Firefox or Safari) and an internet connection. The game loads three.js and a font from a CDN.

### Option 1: open the file

1. Download or clone this repository.
2. Open the project folder.
3. Double-click `index.html`. It opens in your default browser and the game is ready.

### Option 2: run a local server (optional)

1. Open a terminal in the project folder.
2. Start a server with Python:
   ```bash
   python3 -m http.server 8000
   ```
3. Visit `http://localhost:8000` in your browser.

### Clone with Git

```bash
git clone https://github.com/Comelanggilesgiles/snake-3d.git
cd snake-3d
```

## How to play

| Action | Keyboard | Touch |
| --- | --- | --- |
| Start or restart | Space or Enter | Tap the button |
| Move | Arrow keys or WASD | Swipe, or use the d-pad |
| Pause or resume | P or Esc | Tap the button |
| Change camera view | V or the view button | Tap the view button |
| Mute or unmute sound | M or the speaker button | Tap the speaker button |

Eat the amber fruit to grow and score 10 points each time. The game ends if you hit a wall or your own tail.

## Tech stack

- HTML5 and CSS3 for layout and the interface
- JavaScript (vanilla, no framework) for game logic
- [three.js](https://threejs.org/) r128 (WebGL) for 3D rendering
- Web Audio API for sound effects
- localStorage for saving the best score
- Google Fonts: Bricolage Grotesque

## Project structure

```
snake-3d/
  index.html        The whole game: markup, styles and script
  README.md         This file
  docs/
    screenshot.png  Screenshot used in this README
```

## Contributing

Ideas and fixes are welcome. Fork the repository, create a branch, make your change and open a pull request.

## Author

Made by [Comelanggilesgiles](https://github.com/Comelanggilesgiles).
