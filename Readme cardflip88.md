<div align="center">

🃏 CF88

Un jeu de mémoire, cinq ambiances, vos propres symboles.

</div>

---

👋 Welcome

I already made a Memory Match game. Then I made a second one, because the first one wasn't the one I wanted to play.

The first had five themes built on cartoons — SpongeBob, Scooby Doo, Grim, Disney. Loud, colorful, nostalgic. It was fun, but it always felt like it was borrowing its personality from somewhere else. So this version doesn't borrow. Its five themes are its own.

Harvest is a woodblock-print sunflower field at dusk — burnt orange and deep brown, Cinzel for the title, an autumn palette that feels like a print you'd find pinned to a cork board. Midnight is a gothic moonlit night — deep navy, cold blue-grey, one bright yellow accent that cuts through the dark. Noir is red on black, nothing else, all shadow and edge. Whimsical inverts everything into a soft storybook cream with dusty blue and green. And Retro takes the palette of a 1970s poster — teal and ochre and tan, the colors of a beach towel from another decade.

Each one has its own fonts, its own shadows, its own personality. And each one carries the same game underneath: flip pairs of cards, match them, clear the board. There's no image upload here — no base64 bloat in local storage, no awkward resize step. Instead, everything is typed. You write down your own emojis or characters in a text field, press save, and the game uses them. It's lighter than the first version, and it feels more honest. A memory game doesn't need a photo album — it needs a set of small distinct icons, and you already have those on your keyboard.

The default set is sixteen characters with a slightly spooky mood: a fox, a sunflower, a crescent moon, an abandoned house, an eye, a vampire, a spider, a pine tree, a crystal ball, an owl, a bat, a key, a clock, a candle, a coffin, a potion. It fits the Harvest theme's mood without trying too hard — a set of symbols that feel like they belong to a folk tale. You can keep them or replace them entirely with whatever you want: planets, sports, food, initials, Arabic letters, mathematical symbols, ASCII faces. Anything the browser can draw, the game can use.

One HTML file. No account, no timer, no score, no leaderboard. Just the game, the way it was before apps got ideas about what a game should be.

---

<!--
## 📸 Look Inside

<br />

<div align="center">
  <img src="https://github.com/mohamed005cheikh-rgb/cf88/raw/main/images/preview-1.png" alt="The Harvest theme" width="100%" />
  <br />
  <sub><b>① Harvest — the default</b></sub>
</div>

<br />
<br />

<div align="center">
  <img src="https://github.com/mohamed005cheikh-rgb/cf88/raw/main/images/preview-2.png" alt="The Midnight theme" width="100%" />
  <br />
  <sub><b>② Midnight</b></sub>
</div>

<br />
<br />

<div align="center">
  <img src="https://github.com/mohamed005cheikh-rgb/cf88/raw/main/images/preview-3.png" alt="Custom emojis on the board" width="100%" />
  <br />
  <sub><b>③ With your own emojis</b></sub>
</div>
-->

---

✨ What you'll find

Five themes, each one a different room.
The colored dots in the header switch between them instantly, without restarting your game. Harvest — dark brown, burnt orange, Cinzel title, the default. Midnight — deep navy, muted blues, a single bright yellow accent, Special Elite for the title like a typewritten note left on a desk. Noir — the entire screen is black and red, and nothing else. Whimsical — the one light theme: cream background, dusty blue, soft green; a storybook you could read to a child. Retro — teal, ochre, tan; the palette of a poster you'd find in a thrift store. Your choice is saved and remembered.

Three grid sizes.
Eight cards (four pairs), sixteen (eight pairs), or thirty-two (sixteen pairs). The board adapts — 4×2 for the smallest, 4×4 for the middle, 4×8 on desktop for the largest, with a narrower 4×8 on mobile. Changing the size starts a new game automatically.

Three content types.
Numbers — pairs of digits, one through sixteen. Default Emojis — a small curated set of sixteen symbols with a folkloric mood. My Emojis — your own, typed in by hand. Pick the one you want from the content dropdown and the board rebuilds around it.

Your own emojis, in your own words.
The My Emojis field is a plain text input. Type whatever you want, space-separated or comma-separated — 🍕 🍔 🍟 🌮 🍣 🍜 or ❤️ 🧡 💛 💚 💙 💜 or ♠ ♥ ♦ ♣. Press Save My Emojis and the game reloads with your set. Your characters are stored in your browser's local storage, so they persist across sessions. At least four are required so the game always has enough to make pairs.

A 3D flip that feels physical.
Every card uses CSS transform: rotateY(180deg) with preserve-3d and backface-visibility: hidden. The flip takes 0.6 seconds on a cubic-bezier curve that overshoots slightly before settling. The front is what you see before flipping — a decorative patterned back with a subtle compass-rose illustration drawn as inline SVG. The card back is your number, emoji, or character.

Matched cards turn green and get a checkmark.
When two cards match, they don't just stay face-up — they shift to a matched palette (green background, green border), scale down slightly, and gain a small white ✓ in the corner. At a glance, you can see what's been found and what's still waiting, without counting.

A single New Game button.
It reshuffles the board, resets the matched count, and clears the previous state. It doesn't change your theme, your content type, or your custom emojis — it just deals a fresh set. Press it whenever you want a new round.

A Reset Local Data button, for starting clean.
Asks for confirmation, then clears every cf88_* key from local storage: theme, grid size, content type, and custom emojis. Everything returns to defaults — Harvest, sixteen cards, custom emoji mode. Useful when you've saved a set of emojis you're tired of and want the space back.

A win modal that doesn't try too hard.
When the last pair matches, a small modal appears: "Match Found!" as the heading, "You cleared the board perfectly." underneath, and a Play Again button. No confetti, no sound, no timer, no score, no "You beat the world record." Just the small satisfaction of finishing the board.

A vintage grain overlay.
A single SVG noise filter sits over the entire page at 8% opacity, giving every theme a subtly printed texture. It's barely visible in normal use, but it does the work of making the whole thing feel like paper rather than glass.

A monospace footer signature.
Beneath the copyright line at the bottom of the page, a small ASCII block spells out M C 8 8 — the studio mark, rendered in a <pre> tag so it keeps its shape in any monospace font.

Responsive down to a phone.
The header, settings panel, board, and buttons all reflow. The largest grid (thirty-two cards) drops from 8×4 to 4×8 on narrow screens. The font sizes scale with the viewport. The whole thing is designed for a phone screen first, and it looks right on any device.

---

🧭 How it works

1. Open the file.
One HTML file, no build step, no install. The board appears with Harvest and sixteen cards. If you've played before, your last theme, grid size, content type, and custom emojis are restored.

2. Flip a card.
Click or tap any face-down card. It rotates 180 degrees and reveals what's on the back. Flip a second card. If they match — same emoji, same number, same character — they stay face up, turn green, and get a checkmark. If they don't, they flip back after a moment and you try again.

3. Find all the pairs.
Keep going until every card is matched. When the last pair locks in, a modal appears after a short pause. Press Play Again to start a new board with the same settings.

4. Change the theme whenever.
Click one of the five dots in the header. The whole app recolors instantly. Your choice is saved.

5. Change the grid size or content.
Both are in the settings panel below the theme dots. Changing either starts a new game. Your choice is saved.

6. Use your own emojis.
Select My Emojis in the content dropdown. A text field appears. Type your characters, space-separated, and press Save My Emojis. The board reloads with your set. If you haven't saved any yet, the game falls back to the default emojis so the board is never empty.

7. Reset if you want to start over.
The Reset Local Data button at the bottom of the page clears everything after a confirmation prompt. The game returns to its factory defaults.

---

🛠️ A few small helps

"Why isn't there an image upload option?"
Because a previous version of this game had one, and it was heavier than it needed to be. Base64 images fill local storage fast, they're awkward to manage across devices, and a memory game doesn't actually need photographs — it needs distinct, recognizable symbols. Emojis and characters do that job without the weight. If you want the image version, it exists as a separate build.

"Which emojis should I type?"
Anything with visual distinction. Things that look different from each other at a glance. A set of fruit, a set of faces, a set of country flags, a set of geometric symbols, a set of Arabic letters — anything works. The only rule is that at least four of them should be visually distinguishable from each other, so you can tell them apart when they're small and face up on the board.

"My emojis didn't save."
If you're in private browsing mode, localStorage is disabled and nothing persists. Open the file in a normal window and it will save. Also, if you saved emojis, refreshed, and don't see them — check that the content type is still set to My Emojis. The saved set and the content type are separate settings.

"Can I use more emojis than the board needs?"
Yes. If you type thirty emojis and play a sixteen-card game, the game uses the first eight from a shuffled pool. If you type five emojis and play a thirty-two-card game, the game reuses them. Either way it works — it just affects how often the same pair appears.

"Can I use fewer than four?"
No. The Save My Emojis button checks the count and refuses to save if you have fewer than four. Four is the minimum needed for the smallest board to have at least two pairs of distinct symbols.

"Does the game save my progress mid-round?"
No. Every time you reload the file, a new board is dealt. The board state — which cards are flipped, which are matched — is not persisted. Only your settings are.

"What do the numbers on the cards do?"
They're just a content type. If you pick Numbers, each pair shows the same digit — a pair of 1s, a pair of 2s, and so on. It's the simplest, most abstract version of the game, useful as a warm-up or for very young players.

"Why does the card flip feel so smooth?"
Because it uses a real 3D transform with perspective, transform-style: preserve-3d, and backface-visibility: hidden — the same technique used by native apps. The cubic-bezier curve has a slight overshoot, so the card settles into place rather than just stopping.

"How do I make my own theme?"
The CSS has a block for each theme, marked with [data-theme="xxx"]. Copy one, rename it, and adjust the variables — colors, fonts, shadows. Then add a matching <button class="theme-btn xxx" data-theme="xxx"> in the header, plus the matching background color in the .theme-btn.xxx CSS rule. There's no theme counter to update — the buttons just work.

"Does it work offline?"
Almost. The file loads offline, all the game logic runs locally, and your custom emojis are already in local storage. But Google Fonts are loaded from a CDN, so on first launch with no network you'll see fallback system fonts. Load it once with network, and after that it plays fully offline.

"Why does the board sometimes lag when I change grid sizes?"
Because the browser has to destroy and rebuild the entire DOM — every card element is destroyed and recreated. On older devices, that can take a fraction of a second. It's not a bug, it's just the cost of a full reset. Give it a beat and it settles.

"Can I play against someone?"
Not in this version. There's no timer, no turns, no score — it's a solo game. You flip, you match, you clear the board, and that's the whole thing. If you want a two-player mode, that's a different game with different rules.

"What does the ASCII art at the bottom mean?"
It spells M C 8 8 in a blocky font made from █ characters. It's rendered inside a <pre> tag, which is why it keeps its shape — in any monospace font it lines up exactly as written. It's a signature, nothing more.

---

<div align="center">

📞 A question, an idea, a bug?

https://img.shields.io/badge/Email-mohamed005cheikh@gmail.com-d14836?style=flat-square&logo=gmail&logoColor=white
https://img.shields.io/badge/WhatsApp-+222_30_73_64_75-25D366?style=flat-square&logo=whatsapp&logoColor=white
https://img.shields.io/badge/GitHub-mohamed005cheikh--rgb-181717?style=flat-square&logo=github

<br />

Cinq ambiances. Vos symboles. Aucun compte.

<sub>© 2026 Mohamed Cheikh — MC88</sub>

<br />
<br />

</div>ccidental pinch-zooms won't wreck the layout.

"Does it work offline?"
Almost — the file loads offline, and all the game logic runs locally. But the Google Fonts stylesheet is loaded from a CDN, so on first launch with no network you'll see the game in fallback system fonts. Everything else works. Load the file once with network to cache the fonts, and it plays fully offline afterward.

"I want to add a sixth theme."
Look at the [data-theme="disney"] block in the CSS, copy it, rename it, and adjust the variables. Then add a matching <button class="theme-btn yourtheme" data-theme="yourtheme"> in the header, plus the corresponding class in the .theme-btn.xxx rule that sets its dot color. That's the whole ceremony. There's no theme counter to update — the buttons just work.

---

<div align="center">

📞 A question, an idea, a bug?

https://img.shields.io/badge/Email-mohamed005cheikh@gmail.com-d14836?style=flat-square&logo=gmail&logoColor=white
https://img.shields.io/badge/WhatsApp-+222_30_73_64_75-25D366?style=flat-square&logo=whatsapp&logoColor=white
https://img.shields.io/badge/GitHub-mohamed005cheikh--rgb-181717?style=flat-square&logo=github

<br />

Cinq ambiances. Vos images. Aucun compte.

<sub>© 2026 Mohamed Cheikh — MC88</sub>

<br />
<br />

</div>