# Martin92yt — Portfolio

🇫🇷 [Version française](README.md)

My personal portfolio, written **by hand** in pure HTML5 and CSS3: no framework, no library, almost no JavaScript. The site has two pages: the portfolio (`index.html`) and my hardware page (`setup.html`).

Art direction: "artisan-coder". Dark background, orange accent, hand-drawn SVG icons, subtle CSS micro-animations.

## Pages

| Page | File | Content |
|---|---|---|
| Home | `index.html` | About, skills, tools, projects, interests, links, contact |
| Setup | `setup.html` | Desktop PC, laptops, accessories and peripherals |

## Overview

- **About**: introduction and what I build
- **Skills**: TypeScript (main language), HTML5, CSS3, JavaScript, Java, Python, Express.js, EJS, SQLite, JSON
- **Tools**: VS Code, IntelliJ IDEA, Sublime Text, Git & GitHub, HeidSQL, XAMPP, Figma, Trello, Vercel, NPM
- **Projects**: Gifuto, this portfolio and dragons-of-legends.js (see below)
- **Setup**: PC specs (CPU, GPU, RAM, storage…), laptops, monitor, keyboard, mouse, headset, microphone
- **Interests**: video games and anime
- **Links**: Discord, GitHub, YouTube, NPM
- **Contact**: through Discord only

## Featured project: Gifuto

**Gifuto** is a REST API and a community-driven index of anime GIFs, built for Discord bots and web projects. Members can submit, index and categorize GIFs, which can then be used in interaction commands such as `/hug`, `/kiss` or `/pat`.

- **Stack**: Express.js, TypeScript, Prisma, EJS, Neon PostgreSQL
- **Website**: https://gifuto.vercel.app

The portfolio also lists [dragons-of-legends.js](https://www.npmjs.com/package/dragons-of-legends.js), an open source NPM library that simplifies building APIs for MMORPG servers (currently paused).

## Technical highlights

- 100% HTML/CSS: the mobile menu and the modals (legal notice, privacy policy) are driven by `:target`
- Scroll-reveal animations triggered by a tiny `IntersectionObserver` script, identical in every browser (without JavaScript, everything simply stays visible)
- Reading progress bar in pure CSS (`animation-timeline: scroll()`)
- Inline SVG sprite (`<symbol>` + `<use>`) and a "pencil stroke" filter (`feTurbulence` + `feDisplacementMap`)
- Honors `prefers-reduced-motion`
- Responsive from 320 px to 1440 px
- Both pages share the same stylesheet, fonts and hand-drawn icon style
- Fonts and images are served with the site: no third-party service is called when the page loads

## Project structure

```
.
├── index.html        # portfolio
├── setup.html        # hardware / setup page
├── style.css         # shared by both pages
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

## Editing the Setup page

`setup.html` is plain HTML, designed to be edited without breaking the layout. A comment block at the top of the file explains everything. In short:

- **A PC component**: one `<article class="part">` tile (title, main value, optional detail).
- **A monitor**: one `<article class="monitor">` (refresh rate, model, resolution).
- **A peripheral**: one `<article class="gadget">` label (keyboard, mouse, headset, mic, Stream Deck, controller, racing wheel…).

Copy a block to add an item, delete it to remove one.

Rotations, spacing and scroll animations adapt automatically. Components whose model is unknown (case, motherboard, power supply) are simply left out; a commented-out template is ready in the PC section.

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
