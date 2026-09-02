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

## Custom domain

Served at [omostrich.com](https://omostrich.com) via the `CNAME` file in
this repo plus DNS records pointed at GitHub Pages:

- Apex (`omostrich.com`) — four `A` records to `185.199.108.153`,
  `185.199.109.153`, `185.199.110.153`, `185.199.111.153`.
- `www.omostrich.com` — a `CNAME` record to `ninepointlabs.github.io`.

GitHub issues the HTTPS certificate automatically once DNS resolves
correctly; that can take a little while after the records are first added.
