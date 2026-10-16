# AgoraDesktop.github.io

The project website for **[Agora](https://github.com/AgoraDesktop/Agora)** — an installable desktop
environment for Linux and the BSDs.

Published by GitHub Pages from `main` at <https://agoradesktop.github.io> (the organization site —
the repository **name** is what reserves that URL, so it must not change).

## Current state

A placeholder: `index.html` is a self-contained "coming soon" page. Real design and content land
later.

## Layout

| path | purpose |
|---|---|
| `index.html` | The site. Single file — inline CSS, no build step, no external requests. |
| `404.html` | Served by Pages for unknown paths on this site. |
| `favicon.svg` | Site icon. |
| `.nojekyll` | Skip Jekyll; the files are already static. |

## Editing

There is no build step. Edit `index.html` and commit.

Preview locally by opening the file directly, or — to match the deployed server's behaviour,
including `404.html` and absolute paths:

```sh
python3 -m http.server 8000
```

## Design notes

The page is meant to read as a desktop, so it borrows the shell's own vocabulary: a menu bar, a
window with a title bar, and a dock. Everything is one file with no dependencies, and it adapts to
`prefers-color-scheme` (light and dark wallpapers) and `prefers-reduced-motion`.

## Deploying

Pushing to `main` republishes the site automatically.

## Related

- [`AgoraDesktop/.github`](https://github.com/AgoraDesktop/.github) — the organization profile,
  shown at <https://github.com/AgoraDesktop>. This is **not** the website; it only renders on GitHub.
- [`AgoraDesktop/Agora`](https://github.com/AgoraDesktop/Agora) — the development workspace and
  top-level design record.
