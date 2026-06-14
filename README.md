# Panda Deep Dive

An adventure game for kids to practise math. Players guide a panda through the
adventure by solving small equations to set the flight and dive levels —
getting the math right steers how high it flies and how deep it dives.

The entire app ships as one self-contained `index.html`: a React application
bundled inline (markup, styles, and JavaScript all in one file), with a small
loader that unpacks and mounts it. No build step or server is required to view
it — just open the file in a browser.

## Run locally

Open the file directly:

```sh
open index.html
```

Or serve it over HTTP (some browsers restrict features on `file://`):

```sh
python3 -m http.server 8000
# then visit http://localhost:8000
```

## Deploy

The app is a static file, so it can be hosted anywhere that serves static
content. This repo is published with **GitHub Pages** from the `main` branch:

https://thomasbrueggemann.github.io/panda-deep-dive/

## Structure

- `index.html` — the complete application (bundled React app + loader)
