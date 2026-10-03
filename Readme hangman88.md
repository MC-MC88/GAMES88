<div align="center">

🪢 HANGMAN88

Le pendu, en mode paysage. Cinq ciels, deux joueurs, aucune pitié.

</div>

---

👋 Welcome

Le pendu est le premier jeu auquel on joue enfant. Une feuille, un crayon, un mot secret, des traits pour les erreurs. C'est parfait parce que ça ne demande rien — pas de plateau, pas de règles, pas de matériel. Juste deux personnes et un mot.

Et pourtant, toutes les versions numériques que j'ai essayées ont réussi à compliquer ce qui était simple. Un compte pour sauvegarder les scores. Un choix parmi 40 catégories. Un "mode difficile" avec un chronomètre. Des animations à chaque lettre. Des pubs entre deux parties. Quelque part, le pendu est devenu une "expérience" plutôt qu'un jeu.

HANGMAN88 revient à l'essentiel — mais avec un habillage qu'on a envie de regarder.

La forche se dessine en SVG à mesure que vous vous trompez, trait par trait, tête puis corps puis bras puis jambes, dans la couleur d'accent du thème. Les lettres que vous avez déjà essayées se colorent sur le clavier — vert pour correctes, rouge pour fausses. Et surtout, il y a deux modes : jouer contre l'ordinateur avec une banque de 50 mots prédéfinis, ou jouer à deux avec votre propre mot secret, tapé dans un champ, caché à l'écran.

Il y a cinq thèmes, et chacun est un ciel différent. Sunset — un dégradé orange et violet qui descend du haut de l'écran vers un sol jaune paille. Storm — gris-bleu, froid, comme un orage en mer. Midnight — bleu nuit, étoilé, presque noir. Mist — gris doux, une brume d'automne. Ocean — bleu profond et teal vif, l'eau à midi.

Cinq ambiances, un seul jeu, un seul fichier HTML. Pas de compte, pas de score, pas de pub.

---

<!--
## 📸 Look Inside

<br />

<div align="center">
  <img src="https://github.com/mohamed005cheikh-rgb/hangman88/raw/main/images/preview-1.png" alt="The Sunset theme with the setup screen" width="100%" />
  <br />
  <sub><b>① Sunset — the setup screen</b></sub>
</div>

<br />
<br />

<div align="center">
  <img src="https://github.com/mohamed005cheikh-rgb/hangman88/raw/main/images/preview-2.png" alt="The Ocean theme during play" width="100%" />
  <br />
  <sub><b>② Ocean — mid-game</b></sub>
</div>

<br />
<br />

<div align="center">
  <img src="https://github.com/mohamed005cheikh-rgb/hangman88/raw/main/images/preview-3.png" alt="The Midnight theme with the winner modal" width="100%" />
  <br />
  <sub><b>③ Midnight — the winner's modal</b></sub>
</div>
-->

---

✨ What you'll find

Cinq thèmes, cinq ciels.
Les pastilles colorées dans l'en-tête basculent instantanément. Sunset — le défaut. Un dégradé du violet au orange au jaune paille, Cinzel pour le titre, une ambiance de fin de journée en été. Storm — teal froid, gris-bleu, Special Elite à la place de Cinzel, une ambiance d'orage sur la mer. Midnight — bleu nuit presque noir, un seul accent jaune vif, comme une lune sur un ciel sans nuages. Mist — gris doux et bleu pâle, une brume d'automne au bord d'un lac. Ocean — bleu profond avec des accents teal vifs, la couleur de l'eau à midi. Votre choix est sauvegardé, et le prochain lancement démarre déjà dans votre thème.

Deux modes : Bot et Joueur 2.
Le mode Vs Bot pioche un mot au hasard parmi cinquante — animaux, saisons, lieux, métiers, objets. Le mode Vs Player 2 vous laisse taper votre propre mot secret dans un champ, caché derrière la validation. Vous tapez, vous validez, l'écran passe au jeu, et c'est à votre adversaire de deviner. Simple et direct.

Un dessin du pendu qui se construit trait par trait.
La potence (le sol, le poteau, la barre, la corde) est toujours visible. À chaque erreur, une partie du corps apparaît — d'abord la tête, puis le corps, puis les bras, puis les jambes. Six erreurs en tout, six pièces, un dessin complet. Tout est dessiné en SVG, dans la couleur d'accent du thème, avec des traits arrondis.

Un clavier virtuel AZERTY-friendly.
Trois rangées de lettres, QWERTY par ordre alphabétique, chacune avec une ombre portée sous le bouton. Vous cliquez une lettre, elle disparaît du jeu. Correcte : elle devient verte. Fausse : elle devient rouge. Toutes les lettres déjà essayées sont désactivées — impossible de cliquer deux fois sur la même.

Le mot secret avec ses tirets.
Chaque lettre non devinée est un trait sous lequel se cache la réponse. Quand vous trouvez une lettre, elle apparaît au-dessus du trait, dans la couleur d'accent. À la fin de la partie, toutes les lettres sont révélées — même celles que vous n'avez pas trouvées.

Deux indicateurs de partie, sobres.
En haut de l'écran de jeu, un petit tableau noir montre Lives Left (le nombre d'erreurs qu'il vous reste, qui démarre à 6 et descend) et Mode (Bot ou Player 2). Rien d'autre. Pas de score, pas de chronomètre, pas de compteur de coups.

Une modale de fin qui dit tout.
À la fin, une modale apparaît avec Victory! ou Defeat! selon le cas, une phrase adaptée au mode ("You defeated the Bot!" ou "Player 2 guessed it!", "The Bot won this round." ou "Player 2 ran out of lives."), et le mot secret révélé en grosses lettres avec la couleur du résultat — vert pour une victoire, rouge pour une défaite. Un bouton Play Again vous ramène au menu.

Un bouton Quit to Menu pendant la partie.
Vous pouvez abandonner à tout moment et revenir à l'écran de configuration. Pas de confirmation, pas de "êtes-vous sûr de vouloir perdre votre progression" — la partie n'était de toute façon sauvegardée nulle part. C'est un jeu, pas un dossier.

Un grain de film sur tout l'écran.
Un filtre SVG de bruit, appliqué en superposition à 8 % d'opacité, donne à chaque thème une texture imprimée. Ça ne se voit presque pas, mais ça enlève le côté "écran plat" qui aurait rendu le jeu générique.

Une signature ASCII.
Sous le copyright, en bas de page, un petit bloc de caractères dessine M C 8 8 en monospace. C'est la marque du studio, discrète, toujours là.

Responsive, du téléphone à l'écran large.
Le dessin du pendu se redimensionne, le clavier se resserre, les tirets du mot s'adaptent. Toute l'interface est pensée pour un écran de téléphone d'abord, et elle tient aussi très bien sur un écran large.

---

🧭 Comment ça marche

1. Ouvrez le fichier.
Un seul HTML, pas de build, pas d'installation. L'écran de configuration apparaît avec le thème Sunset et deux choix de mode.

2. Choisissez un mode.
Cliquez sur Vs Bot pour jouer contre l'ordinateur — un mot est tiré au hasard, et vous commencez à deviner. Ou cliquez sur Vs Player 2 pour taper votre propre mot secret — un champ apparaît, vous tapez, vous validez, l'écran passe à la partie.

3. Devinez les lettres.
Cliquez sur les lettres du clavier virtuel. Correctes, elles s'affichent dans le mot et deviennent vertes. Fausses, elles deviennent rouges et une partie du corps se dessine. Six erreurs et la partie est perdue.

4. Trouvez le mot, ou non.
Quand toutes les lettres du mot sont devinées, la modale de victoire apparaît. Quand six erreurs sont commises, la modale de défaite apparaît avec le mot révélé. Dans les deux cas, un bouton Play Again vous ramène au menu.

5. Changez de thème si l'envie vous prend.
Les cinq pastilles dans l'en-tête. Le clic change tout instantanément, y compris la couleur de la potence et des traits du dessin. Votre choix est sauvegardé pour la prochaine fois.

6. Recommencez autant de fois que vous voulez.
Le bouton Quit to Menu pendant la partie. Un nouveau clic sur Start régénère un nouveau mot ou attend votre prochaine saisie. Pas de limite, pas de compteur.

---

🛠️ A few small helps

"Puis-je utiliser des mots avec des espaces ou des accents ?"
Non. Le jeu n'accepte que des lettres A à Z, sans espace, sans accent, sans tiret. Si vous tapez autre chose, la validation vous refuse avec un message d'erreur. Utilisez des mots simples, en majuscules ou en minuscules (le jeu convertit tout en majuscules de toute façon).

"Puis-je entrer un mot de moins de trois lettres ?"
Non. Le jeu exige un minimum de trois lettres pour éviter les parties triviales. Un mot de trois lettres est déjà très court, mais c'est autorisé. En dessous, le message d'erreur vous en empêche.

"Que se passe-t-il si deux joueurs veulent rejouer ?"
Le bouton Play Again vous ramène au menu. Choisissez le mode à nouveau, et si c'est en PvP, tapez un nouveau mot. Il n'y a pas de mémorisation — chaque partie repart de zéro.

"Le mot secret est-il visible quelque part pendant la partie ?"
Non. Une fois que vous avez validé votre mot en mode PvP, le champ est vidé, et le mot est stocké uniquement en mémoire JavaScript côté navigateur. Rien n'est sauvegardé, rien n'est envoyé nulle part. Un adversaire curieux ne peut pas le retrouver dans le HTML ou dans localStorage.

"La banque de mots contient combien de mots, et lesquels ?"
Cinquante mots, tous en anglais, sans accents, choisis pour être faciles à reconnaître. Des animaux, des saisons, des lieux, des métiers, des objets, des personnages de fiction. Vous pouvez les voir dans le code source, dans le tableau WORD_BANK. Si vous voulez ajouter les vôtres, ouvrez le fichier dans un éditeur et ajoutez-les à la liste.

"Puis-je ajouter mes propres mots au mode Bot ?"
Oui. Ouvrez le fichier, cherchez const WORD_BANK = [, et ajoutez vos mots entre guillemets, séparés par des virgules. Chaque mot doit être en majuscules sans accents pour fonctionner correctement avec le clavier virtuel.

"Le thème est-il sauvegardé ?"
Oui. Le thème que vous choisissez est conservé dans localStorage sous la clé hangman88_theme, et le prochain lancement démarre déjà dedans. En navigation privée, localStorage est désactivé et le thème reviendra à Sunset à chaque ouverture.

"Est-ce que la partie est sauvegardée si je ferme la page ?"
Non. Rien n'est conservé — ni le mot secret, ni les lettres déjà devinées, ni le nombre d'erreurs. Chaque ouverture repart d'un menu frais. C'est un jeu, pas un dossier.

"Puis-je jouer avec le clavier de mon ordinateur ?"
Pas directement dans cette version. Le clavier virtuel à l'écran est le seul moyen de saisir une lettre. C'est un choix délibéré — l'app est pensée pour un usage tactile sur téléphone, et ajouter des raccourcis clavier aurait compliqué l'interface. Si vous voulez l'ajouter, l'écouteur d'événements est un keydown à poser sur document, en filtrant sur les lettres A à Z.

"Est-ce que ça marche hors ligne ?"
Oui, entièrement. Les polices Google Fonts (Cinzel, Nunito, Special Elite) sont chargées depuis un CDN, donc lors du tout premier lancement avec une connexion vous les verrez arriver. Après ce premier chargement, tout fonctionne hors ligne — le dessin SVG, la logique du jeu, les animations, tout est local.

"Pourquoi six erreurs et pas dix ou cinq ?"
Six, c'est le standard classique du pendu — juste assez pour que le dessin ait un sens (tête, corps, deux bras, deux jambes) et juste assez court pour que la tension monte après trois erreurs. Cinq, on perd trop vite. Dix, on ne perd jamais.

"Puis-je modifier le nombre d'erreurs autorisées ?"
Oui. Ouvrez le fichier, cherchez const MAX_WRONG = 6; et changez la valeur. Attention : les six parties du dessin correspondent aux six erreurs. Si vous mettez moins, certaines parties ne s'afficheront jamais. Si vous mettez plus, les erreurs supplémentaires n'auront plus de dessin à ajouter — elles compteront quand même dans le total, mais le pendu sera déjà complet.

"Puis-je changer les couleurs d'un thème ?"
Oui, dans le CSS. Chaque thème est un bloc [data-theme="xxx"] qui définit des variables. Copiez un bloc, renommez-le, ajustez les valeurs. Ajoutez ensuite un bouton correspondant dans l'en-tête et une règle .theme-btn.xxx pour sa couleur. Il n'y a pas de compteur à mettre à jour.

"Pourquoi le clavier n'affiche-t-il que 26 lettres, pas de Ç ou de Ñ ?"
Parce que le jeu est en anglais et la banque de mots ne contient que des mots anglais. Ajouter des caractères accentués serait possible en modifiant à la fois le clavier virtuel et la banque de mots, mais ça aurait compliqué la validation. Si vous jouez en français, restez sur des mots sans accents — "CHAT", "MAISON", "ARBRE", "LIVRE" — et tout fonctionne.

---

<div align="center">

📞 Une question, une idée, un bug ?

https://img.shields.io/badge/Email-mohamed005cheikh@gmail.com-d14836?style=flat-square&logo=gmail&logoColor=white
https://img.shields.io/badge/WhatsApp-+222_30_73_64_75-25D366?style=flat-square&logo=whatsapp&logoColor=white
https://img.shields.io/badge/GitHub-mohamed005cheikh--rgb-181717?style=flat-square&logo=github

<br />

Cinq ciels. Deux joueurs. Aucune pitié.

<sub>© 2026 Mohamed Cheikh — MC88</sub>

<br />
<br />

</div>