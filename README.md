<p align="center"><img src="docs/banner.svg" alt="Hammer & Ember themed project banner" width="100%"></p>

# Hammer & Ember

*Every blade is folded 512 times*

A bladesmith atelier concept set around the making of a single pattern-welded sword. Coal, steel, heat, and patient handwork replace a conventional product catalogue.

The project is live at `https://ember.aarya.cyou/`. The site is an interactive concept; its booking, purchase, or application invitations do not complete real transactions.

## The idea

This project treats craft as an atmosphere to enter. Its selected scenes move from **Two steels** to **The finish**, giving the central subject several different scales and moods. The result is a designed world rather than a catalogue of screens.

<p align="center"><img src="docs/chapters.svg" alt="Four themed chapters from Hammer & Ember" width="100%"></p>

## Four scenes

| No. | Scene | Place in the story |
| --- | --- | --- |
| 1 | **Two steels** | The billet begins as a deliberate pairing. |
| 2 | **The strike** | Orange heat becomes shape under the hammer. |
| 3 | **The quench** | A brief moment fixes the blade. |
| 4 | **The finish** | Polish and acid reveal the pattern. |

These scenes are a selection from the full site. The page also contains supporting editorial sections and a closing invitation.

## Visual language

Soot black, ember orange, bone text, and a condensed display face carry the temperature of the forge.

The color plate below records the project's ground, ink, accent, and secondary tone. The type families in the design are Oswald · Crimson Pro.

<p align="center"><img src="docs/palette.svg" alt="Hammer & Ember color and typography plate" width="100%"></p>

## The site

The experience is built for the browser, with a visual scene that responds to the page and pointer. Its text remains arranged as a readable sequence of sections. The screenshot below shows the opening composition.

<p align="center"><img src="docs/media/ember.webp" alt="Opening screen of the Hammer & Ember website" width="100%"></p>

<p align="center"><sub>Opening scene captured from the original project.</sub></p>

## Built with

| Part | Tools |
| --- | --- |
| Site and build | JavaScript, Vite, Tailwind CSS, custom CSS |
| Three-dimensional scene | Three.js and project-specific shaders/models |
| Motion and scrolling | GSAP, ScrollTrigger, Lenis |
| Hosting configuration | Cloudflare Pages, `wrangler.jsonc` |

The site is one project at the repository root. The current application is in `src/`; render, asset, input, scroll, and UI utilities are in `src/core/`. Old collection material is preserved under `docs/archive/`.

## Run locally

Use Node.js 22.12 or newer:

```bash
npm ci
npm run dev
```

Vite serves the site at `http://127.0.0.1:5190/`. To build and preview the production output:

```bash
npm run build
npm run preview
```

The build writes to `dist/`; preview serves it at `http://127.0.0.1:5191/`.

## Deployment

For Cloudflare Pages, connect the repository's `main` branch. Use `npm run build` as the build command, `dist` as the output directory, and the repository root as the root directory. The React (Vite) preset supplies the build values; `wrangler.jsonc` also records the Pages output directory. The live site is `https://ember.aarya.cyou/`; pushes to `main` deploy through the connected GitHub repository.

## Repository guide

| Path | Contents |
| --- | --- |
| `index.html` | Single site entry |
| `src/` | Scene, styles, shaders, and page modules |
| `src/core/` | Shared rendering and interaction utilities |
| `public/` | Project models and images |
| `docs/` | Project art, screenshot, credits, and notices |
| `docs/archive/` | Preserved earlier collection material |
| `wrangler.jsonc` | Cloudflare Pages output configuration |

## Rights and credits

The repository has separate rights scopes. Reuse rights for one part do not extend to the others:

| Material | Terms |
| --- | --- |
| Adapted source code | [MIT license](LICENSE), with the original copyright retained |
| New project SVGs and original presentation | [Hammer & Ember content notice](LICENSE-EMBER.md) |
| Zyrix Dev name and marks, where referenced | [Zyrix Dev brand notice](LICENSE-ZYRIXDEV.md) |
| Models, source images, and the screenshot | [Asset licenses](docs/ASSET-LICENSES.md) |
| Libraries and web fonts | [Third-party notices](docs/THIRD-PARTY-NOTICES.md) |

The source project and contributors are acknowledged in [Credits](docs/CREDITS.md). The original source copyright remains in [LICENSE](LICENSE).
