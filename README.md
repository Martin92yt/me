# Martin92yt — Portfolio

🇫🇷 [Version française](README.md)

My personal portfolio, written **by hand** in pure HTML5 and CSS3: no framework, no library, almost no JavaScript.

Art direction: "artisan-coder". Dark background, orange accent, hand-drawn SVG icons, subtle CSS micro-animations.

## Overview

- **About**: introduction and what I build
- **Skills**: TypeScript (main language), HTML5, CSS3, JavaScript, Java, Python, Express.js, EJS, SQLite, JSON
- **Tools**: VS Code, IntelliJ IDEA, Sublime Text, Git & GitHub, HeidSQL, XAMPP, Figma, Trello, Vercel, NPM
- **Projects**: [dragons-of-legends.js](https://www.npmjs.com/package/dragons-of-legends.js) and this portfolio
- **Interests**: video games and anime
- **Links**: Discord, GitHub, YouTube, NPM
- **Contact**: through Discord only

## Technical highlights

- 100% HTML/CSS: the mobile menu and the modals (legal notice, privacy policy) are driven by `:target`
- Scroll-reveal animations using `animation-timeline: view()`, with a tiny `IntersectionObserver` fallback for browsers that don't support it
- Reading progress bar in pure CSS (`animation-timeline: scroll()`)
- Inline SVG sprite (`<symbol>` + `<use>`) and a "pencil stroke" filter (`feTurbulence` + `feDisplacementMap`)
- Honors `prefers-reduced-motion`
- Responsive from 320 px to 1440 px
- Fonts and images are served with the site: no third-party service is called when the page loads

## Project structure

```
.
├── index.html
├── style.css
├── LICENSE
├── README.md
├── README.en.md
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

## Run locally

No installation needed: open `index.html` in a browser.

To get the same behavior as in production, you can also serve the folder:

```bash
npx serve .
```

## Deployment

The site is static and hosted on [Vercel](https://vercel.com). No build step is required; `index.html` sits at the root.

## Fonts

[Fraunces](https://fonts.google.com/specimen/Fraunces), [Caveat](https://fonts.google.com/specimen/Caveat) and [Space Mono](https://fonts.google.com/specimen/Space+Mono), licensed under the [SIL Open Font License 1.1](https://openfontlicense.org/).

## License and rights

- **Code (HTML/CSS)**: [MIT License](LICENSE)
- **Text content**: © Martin92yt, all rights reserved
- **Avatar**: an item from the Steam store, legally purchased; it is not my own creation and is not covered by the MIT license
- **Game visuals**: property of their respective publishers (Mojang Studios / Microsoft, Coffee Stain Studios, Unknown Worlds Entertainment, HoYoverse), used for illustration purposes only

## Contact

Via Discord: `.player_green`