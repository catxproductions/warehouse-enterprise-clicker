# Warehouse Enterprise Clicker

A self-contained clicker/idle game. `index.html` is the whole game — no
build step, no server, saves to the browser's `localStorage`.

## Deploying on GitHub Pages

1. Push this folder's contents to a GitHub repo (the two files `index.html`
   and `download.html`, plus `.nojekyll`, should sit at the repo root or in
   whichever folder you point Pages at).
2. In the repo, go to **Settings → Pages**.
3. Under **Build and deployment → Source**, choose **Deploy from a branch**.
4. Pick your branch (e.g. `main`) and the folder (`/root`, or `/docs` if you
   put the files there instead), then **Save**.
5. GitHub will publish the site at `https://<username>.github.io/<repo>/`
   (or `https://<username>.github.io/` if the repo is named
   `<username>.github.io`). It can take a minute or two after the first push.

The `.nojekyll` file tells GitHub Pages to serve everything as plain static
files rather than running it through Jekyll — not needed for this game, but
it's what Jekyll would otherwise ignore or mangle.

`unused-netlify-backend/` and `LEGACY DONT TOUCH/` are not part of the live
site; GitHub Pages will happily ignore them since nothing links to their
contents.
