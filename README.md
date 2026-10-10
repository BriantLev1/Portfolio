# WDD 331R Portfolio

**Student:** Briant Woolley
**Semester:** Fall semester of 2026
**Live Site:** [View Site](https://briantlev1.github.io/Portfolio/)

## About

This repository is my portfolio for WDD 331R: Advanced CSS.
Each week I add new pages and styles as I work through the course
assignments. The site deploys automatically to GitHub Pages on
every push to main.

## Pages

- [Home](index.html)
- [Custom Properties and Nesting](unit-1/custom-properties/index.html)
- [Layered Components](unit-2/layered-components/index.html)
- [::part() and ::slotted()](unit-2/part-and-slotted/index.html)

## Project Structure

```
Portfolio/
├── css/
│   ├── base/
│   │   ├── elements.css      # Bare element styles (body, headings, links)
│   │   └── reset.css         # Minimal CSS reset
│   ├── components/
│   │   └── card.css          # .card component
│   ├── layout/
│   │   └── primary.css       # Page skeleton: header, card grid, footer
│   ├── tokens/
│   │   ├── colors.css        # Color custom properties
│   │   └── variables.css     # Spacing, typography, radius, and other tokens
│   ├── utilities/
│   │   └── utilities.css     # Single-purpose helpers (.visually-hidden, .text-center)
│   └── main.css              # Entry point: declares layer order and imports every file
├── dist/
│   └── styles.css            # Bundled, minified build output (committed on purpose)
├── unit-1/                   # Unit 1 assignments
├── unit-2/                   # Unit 2 assignments and choose topics
├── index.html                # Homepage
├── package.json              # Build script and dev dependency
└── README.md
```

## CSS Architecture

The CSS follows a layered, token-first architecture. `css/main.css` is the single
entry point. It declares the cascade order first, then imports each file into its layer:

```css
@layer tokens, base, layout, components, utilities;
```

Later layers beat earlier ones regardless of selector specificity, so utilities can
override components without `!important`.

| Layer | Folder | What belongs there |
| --- | --- | --- |
| `tokens` | `css/tokens/` | Custom properties for every design decision |
| `base` | `css/base/` | The reset and bare HTML element styles |
| `layout` | `css/layout/` | Page structure and composition |
| `components` | `css/components/` | Styled UI pieces such as cards |
| `utilities` | `css/utilities/` | Small helper classes |

**Token-first:** colors live in `tokens/colors.css`, and everything else (spacing,
typography, border radius) lives in `tokens/variables.css`. Other files reference
tokens with `var()` instead of typing raw values.

**Adding a new file:** create it in the right folder, then add one `@import` line to
`css/main.css` with the matching `layer()` assignment.

## Build Tool

I chose [Lightning CSS](https://lightningcss.dev/). It bundles the `@import` files
in `css/main.css` into one file and minifies the result.

### How to run the build

You need [Node.js](https://nodejs.org/) installed.

```
npm install
npm run build
```

The build script in `package.json` is:

```
lightningcss --minify --bundle css/main.css -o dist/styles.css
```

It reads `css/main.css` and writes the bundled, minified output to
`dist/styles.css`. If `dist/` does not exist yet, create it first with `mkdir dist`.

`dist/styles.css` is committed to the repository so the bundler output can be
reviewed. `node_modules/` is ignored by `.gitignore`. The homepage links to
`css/main.css` directly, so the layered source files are what the browser loads.