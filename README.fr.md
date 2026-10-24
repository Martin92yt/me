# Martin92yt — Portfolio

🇬🇧 [English version](README.en.md)

Mon portfolio personnel, écrit **à la main** en HTML5 et CSS3 pur : pas de framework, pas de bibliothèque, presque pas de JavaScript.

Direction artistique « artisan-coder » : fond sombre, accent orange, icônes SVG dessinées à la main, petites animations CSS discrètes.

## Aperçu

- **À propos** : présentation et ce que je construis
- **Compétences** : TypeScript (langage principal), HTML5, CSS3, JavaScript, Java, Python, Express.js, EJS, SQLite, JSON
- **Outils** : VS Code, IntelliJ IDEA, Sublime Text, Git & GitHub, HeidSQL, XAMPP, Figma, Trello, Vercel, NPM
- **Projets** : [dragons-of-legends.js](https://www.npmjs.com/package/dragons-of-legends.js) et ce portfolio
- **Passions** : jeux vidéo et animes
- **Réseaux** : Discord, GitHub, YouTube, NPM
- **Contact** : uniquement via Discord

## Particularités techniques

- 100 % HTML/CSS : menu mobile et fenêtres modales (mentions légales, confidentialité) gérés avec `:target`
- Animations à l'apparition via `animation-timeline: view()`, avec un petit script de secours (`IntersectionObserver`) pour les navigateurs qui ne le gèrent pas
- Barre de progression de lecture en CSS (`animation-timeline: scroll()`)
- Sprite SVG inline (`<symbol>` + `<use>`) et filtre « trait de crayon » (`feTurbulence` + `feDisplacementMap`)
- Respect de `prefers-reduced-motion`
- Responsive de 320 px à 1440 px
- Polices et images hébergées avec le site : aucun service tiers n'est appelé au chargement

## Structure

```
.
├── index.html
├── style.css
├── LICENSE
├── README.md
├── fonts/
│   ├── Caveat.ttf
│   ├── Fraunces.ttf
│   ├── SpaceMono-Regular.ttf
│   └── SpaceMono-Bold.ttf
└── images/
    ├── avatar.jpg
    ├── minecraft.jpg
    ├── satisfactory.jpg
    ├── subnautica.jpg
    └── genshin-impact.jpg
```

## Lancer en local

Aucune installation : ouvrir `index.html` dans un navigateur.

Pour un rendu identique à la production, on peut aussi servir le dossier :

```bash
npx serve .
```

## Déploiement

Le site est statique et hébergé sur [Vercel](https://vercel.com) : aucune commande de build n'est nécessaire, `index.html` est à la racine.

## Polices

[Fraunces](https://fonts.google.com/specimen/Fraunces), [Caveat](https://fonts.google.com/specimen/Caveat) et [Space Mono](https://fonts.google.com/specimen/Space+Mono), sous licence [SIL Open Font License 1.1](https://openfontlicense.org/).

## Licence et droits

- **Code (HTML/CSS)** : [licence MIT](LICENSE)
- **Textes** : © Martin92yt, tous droits réservés
- **Avatar** : objet de la boutique Steam, acquis légalement ; il n'est pas ma création et n'est pas couvert par la licence MIT
- **Visuels de jeux** : propriété de leurs éditeurs respectifs (Mojang Studios / Microsoft, Coffee Stain Studios, Unknown Worlds Entertainment, HoYoverse), utilisés à titre illustratif uniquement

## Contact

Via Discord : `.player_green`