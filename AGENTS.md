# Agent notes

- Dependency-free static game: `index.html` loads all logic from `game.js`. There is no package manager, build, lint, or automated test suite — verify changes by playing in a browser.
- Run by opening `index.html` or with `npx serve .` (then visit `http://localhost:3000`). UI text and controls are in Spanish.
- `game.js` is a classic script (no `type="module"`): it uses global scope, so do not add `import`/`export`.
- Input has two paths: `keys` tracks held keys, while `pressed()` consumes one-shot presses. Use `pressed()` for actions like shooting/restart, not `keys`.
- The 800×600 canvas size is duplicated in `index.html` and `game.js` (`W`/`H`); update both when changing the playfield.
- README must stay in sync with `game.js`. Currently the only power-up implemented is "Velocidad"; there is no "estrella fugaz" asteroid. Trust the code over the README if they disagree.
