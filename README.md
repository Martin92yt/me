# Martin92yt — Portfolio

🇫🇷 [Version française](README.fr.md)

My personal portfolio, written **by hand** in pure HTML5 and CSS3: no framework, no library, almost no JavaScript.

Art direction: "artisan-coder". Dark background, orange accent, hand-drawn SVG icons, subtle CSS micro-animations.

## Pages

| Page | File | Content |
|---|---|---|
| Home | `index.html` | About, skills, tools, a preview of my projects, interests, links, contact |
| Projects | `projets.html` | Detailed case studies: description, tech stack, screenshots and links (npm, GitHub, live site) |
| Setup | `setup.html` | PC specs, monitors, peripherals, and my other machines |

## Featured projects

### Gifuto

A REST API and a community-driven index of anime GIFs, built for Discord bots and web projects. Members submit GIFs, which are then indexed and categorized so they can be used in interaction commands such as `/hug`, `/kiss` or `/pat`.

- **Stack**: TypeScript, Express.js, Prisma, EJS, Neon PostgreSQL
- **Website**: https://gifuto.vercel.app
- **npm package**: [`gifuto.js`](https://www.npmjs.com/package/gifuto.js), which reached 300 downloads in a single day

### dragons-of-legends.js

An open source NPM library that simplifies building APIs for MMORPG servers, written in TypeScript. It has more than 2,900 downloads.

- **npm**: https://www.npmjs.com/package/dragons-of-legends.js
- **Repository**: https://github.com/Martin92yt/DragonsOfLegends.js

### This portfolio

Hand-coded in HTML and CSS, focused on minimalism and performance. Source code: https://github.com/Martin92yt/me

## Technical highlights

- 100% HTML/CSS: the mobile menu and the modals (legal notice, privacy policy) are driven by `:target`
- Scroll-reveal animations triggered by a tiny `IntersectionObserver` script, identical in every browser (without JavaScript, everything simply stays visible)
- Reading progress bar in pure CSS (`animation-timeline: scroll()`)
- Inline SVG sprite (`<symbol>` + `<use>`) and a "pencil stroke" filter (`feTurbulence` + `feDisplacementMap`)
- Honors `prefers-reduced-motion`
- Responsive from 320 px to 1440 px
- All pages share the same stylesheet, fonts and hand-drawn icon style
- Fonts and images are served with the site: no third-party service is called when a page loads

## Project structure

```
.
├── index.html          # home
├── projets.html        # projects
├── setup.html          # hardware / setup
├── 404.html            # not-found page (served by Vercel)
├── style.css           # shared by all pages
├── LICENSE
├── README.md           # English (default)
├── README.fr.md        # French
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

## Editing the content

Both `projets.html` and `setup.html` are plain HTML designed to be edited without breaking the layout. A comment block at the top of each file explains how.

- **Projects page**: one `<article class="case">` per project. Copy a block to add a project, delete it to remove one. Each line of the "In short" and "Stack" lists is a `<li>` to copy, edit or delete. Drop the screenshots in `images/projects/` (16:10 ratio recommended); a drawn placeholder shows until the file exists.
- **Setup page**: one `<article class="part">` per PC component, `monitor` per screen, `gadget` per peripheral and `device` per machine.

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
