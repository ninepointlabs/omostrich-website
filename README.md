# omostrich-website

Source for the Omostrich landing page, published via GitHub Pages.

Plain HTML/CSS, no build step — `index.html` plus `assets/`. Explains
[Omostrich](https://github.com/ninepointlabs/omostrich) (the Nostr
signer/composer for the Omarchy desktop) and its optional sibling
[Omostrich-DB](https://github.com/ninepointlabs/omostrich-db) in plain
language, styled in the same dark terminal palette as
[omarchy.org](https://omarchy.org).

## Local preview

```bash
python3 -m http.server 8000
```

then open `http://localhost:8000`.

## Deploy

GitHub Pages is configured to serve from the `main` branch root — push to
`main` and the site updates automatically.
