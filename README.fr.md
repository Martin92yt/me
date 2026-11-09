# Martin92yt — Portfolio

🇬🇧 [English version](README.md)

Mon portfolio personnel, écrit **à la main** en HTML5 et CSS3 pur : pas de framework, pas de bibliothèque, presque pas de JavaScript.

Direction artistique « artisan-coder » : fond sombre, accent orange, icônes SVG dessinées à la main, petites animations CSS discrètes.

## Pages

| Page | Fichier | Contenu |
|---|---|---|
| Accueil | `index.html` | À propos, compétences, outils, aperçu des projets, passions, réseaux, contact |
| Projets | `projets.html` | Études détaillées : description, stack technique, captures d'écran et liens (npm, GitHub, site) |
| Setup | `setup.html` | PC, écrans, périphériques et mes autres machines |

## Projets à la une

### Gifuto

Une API REST et un indexeur communautaire de GIFs d'anime, pensé pour les bots Discord et les projets web. La communauté soumet des GIFs, qui sont ensuite indexés et catégorisés pour des commandes comme `/hug`, `/kiss` ou `/pat`.

- **Stack** : TypeScript, Express.js, Prisma, EJS, Neon PostgreSQL
- **Site** : https://gifuto.vercel.app
- **Package npm** : [`gifuto.js`](https://www.npmjs.com/package/gifuto.js), qui a atteint 300 téléchargements en une seule journée

### dragons-of-legends.js

Une librairie NPM open source qui simplifie la création d'APIs pour serveurs MMORPG, écrite en TypeScript. Plus de 2 500 téléchargements.

- **npm** : https://www.npmjs.com/package/dragons-of-legends.js
- **Dépôt** : https://github.com/Martin92yt/DragonsOfLegends.js

### Ce portfolio

Codé à la main en HTML et CSS, axé sur le minimalisme et la performance. Code source : https://github.com/Martin92yt/me

## Particularités techniques

- 100 % HTML/CSS : menu mobile et fenêtres modales (mentions légales, confidentialité) gérés avec `:target`
- Animations à l'apparition déclenchées par un petit script `IntersectionObserver`, identique sur tous les navigateurs (sans JavaScript, tout reste simplement visible)
- Barre de progression de lecture en CSS (`animation-timeline: scroll()`)
- Sprite SVG inline (`<symbol>` + `<use>`) et filtre « trait de crayon » (`feTurbulence` + `feDisplacementMap`)
- Respect de `prefers-reduced-motion`
- Responsive de 320 px à 1440 px
- Toutes les pages partagent la même feuille de style, les mêmes polices et le même style d'icônes
- Polices et images hébergées avec le site : aucun service tiers n'est appelé au chargement

## Structure

```
.
├── index.html          # accueil
├── projets.html        # projets
├── setup.html          # matériel
├── style.css           # commun à toutes les pages
├── LICENSE
├── README.md           # anglais (par défaut)
├── README.fr.md        # français
├── fonts/
│   ├── Caveat.ttf
│   ├── Fraunces.ttf
│   ├── SpaceMono-Regular.ttf
│   └── SpaceMono-Bold.ttf
└── images/
    ├── avatar.gif
    ├── minecraft.jpg
    ├── satisfactory.jpg
    ├── subnautica.jpg
    ├── genshin-impact.jpg
    └── projects/
        ├── gifuto.png
        ├── dragons-of-legends.png
        └── portfolio.png
```

## Modifier le contenu

`projets.html` et `setup.html` sont du HTML simple, pensé pour être modifié sans casser le design. Un bloc de commentaires en haut de chaque fichier explique comment faire.

- **Page Projets** : un `<article class="case">` par projet. On copie un bloc pour ajouter un projet, on le supprime pour l'enlever. Chaque ligne des listes « En bref » et « Stack » est un `<li>` à copier, modifier ou supprimer. Les captures vont dans `images/projects/` (format 16:10 conseillé) ; un dessin de remplacement s'affiche tant que le fichier n'existe pas.
- **Page Setup** : un `<article class="part">` par composant du PC, `monitor` par écran, `gadget` par périphérique et `device` par machine.

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