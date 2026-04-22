# enfilade.io

Static site for Enfilade, served via GitHub Pages.

## Structure

- `index.html` — single page
- `style.css` — styles
- `assets/` — logos, PGP public key
- `CNAME` — custom domain (enfilade.io)

## Local preview

```
python3 -m http.server 8000
```

Then open http://localhost:8000.

## Deploy

Push to `main`. GitHub Pages serves `/` from the branch root.

## Before launch

- Replace the fingerprint placeholder in `index.html` with the real PGP fingerprint.
- Drop the PGP public key at `assets/enfilade-pgp.asc`.
- Confirm DNS is pointed at GitHub Pages (see `DOMAIN.md`).
