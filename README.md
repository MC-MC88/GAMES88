```markdown
<div align="center">

# 🎮 Games88

**A single page that gathers all the games.**

</div>

---

## What it is

Games88 is a hub page. It opens on a wall of posters — one for each game — and clicking a poster takes you to that game. No menus, no account, no installation. One page, several games.

Each game lives in its own HTML file, independent, and works on its own. Games88 just gathers them in one place.

---

## Games in this collection

| # | Game | Category | File |
|---|------|----------|------|
| 01 | Card Flip | Memory | `CF.html` |
| 02 | Rock Paper Scissors | Reflex | `RPS88.html` |
| 03 | Hangman | Word | `hangman88.html` |
| 04 | Numbrle | Numbers | `numbrel88.html` |
| 05 | Simon Says | Sequence | `simon says vol2.html` |
| 06 | Sudoku | Logic | `sudoku88.html` |

Each game has its own README in its own repository, with full documentation, features, and notes.

---

## How to use

Open `index.html` in a browser. Click any poster. The game opens in the same tab.

To go back to the hub from any game, use the browser's back button.

---

## Structure

The project expects all files in the same folder:

```

GAMES88/
├── index.html              ← hub page
├── CF.html
├── RPS88.html
├── hangman88.html
├── numbrel88.html
├── simon says vol2.html
├── sudoku88.html
└── README.md

```

No dependencies. No build step. No server. Open the file, it works.

---

## Adding a game

To add a new game to the hub, open `index.html` and copy one of the existing `<a class="poster">` blocks. Change the `href` to the file name, the title, the icon, the description, and the category.

Available categories (they set the poster color):
`memory` · `reflex` · `word` · `numbers` · `sequence` · `logic`

---

## License

MIT. Free to use, modify, and share, with the original copyright preserved.

---

<div align="center">

[![Email](https://img.shields.io/badge/Email-mohamed005cheikh@gmail.com-d14836?style=flat-square&logo=gmail&logoColor=white)](mailto:mohamed005cheikh@gmail.com)
[![GitHub](https://img.shields.io/badge/GitHub-MC--MC88-181717?style=flat-square&logo=github)](https://github.com/MC-MC88)

<sub>© 2026 Mohamed Cheikh — MC88</sub>

</div>
```
