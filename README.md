# Xbox

> **Created: February 2022** — learning project (first steps with a Sass/SCSS workflow).

An Xbox-themed landing page. The main goal of this one was learning to work with **Sass (SCSS)** — splitting styles into partials and compiling them to CSS — on top of Bootstrap 5.

The page currently focuses on the **header / navigation bar**; it was a work in progress.

## What's built

- A responsive **Bootstrap 5 navbar**: Xbox logo, nav links (Games, Consoles, a Community dropdown), a search field, and a "My XBOX" dropdown, with a collapsible burger menu on small screens.
- Custom dark theme and nav-link hover/active states via SCSS.
- Self-hosted **Helvetica Neue** font kit (`@font-face`, multiple weights/styles).

## SCSS structure

Styles are organized as partials imported from `scss/style.scss`:

| Partial            | Purpose |
|--------------------|---------|
| `_variebles.scss`  | Variables (e.g. background color). |
| `_assets.scss`     | Base/body styles using the variables. |
| `_header.scss`     | Header and navbar styling. |

These compile to `scss/style.css` (with a `.css.map` source map).

## Running

Open `index.html` in a browser. To change styles, edit the `.scss` files and recompile with Sass:

```bash
sass scss/style.scss scss/style.css
```

## Stack

- HTML / CSS
- Sass (SCSS)
- Bootstrap 5
