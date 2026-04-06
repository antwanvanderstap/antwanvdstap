# antwanvanderstap.github.io

Personal website for Antwan van der Stap, prepared for GitHub Pages with a custom domain.

## Files

- `index.html`: homepage
- `resume.html`: printable resume page
- `assets/site.css`: shared site styling
- `404.html`: custom not found page
- `CNAME`: custom domain for GitHub Pages
- `.nojekyll`: serves the site as a plain static project

## Local Preview

From this folder:

```bash
python3 -m http.server 8080
```

Then open `http://localhost:8080`.

## Recommended GitHub Setup

1. Create a new public repository named `antwanvanderstap.github.io`.
2. Push this folder to the `main` branch of that repository.
3. In GitHub, open `Settings -> Pages` and confirm the site is publishing from the `main` branch root.
4. Keep the included `CNAME` file so GitHub Pages serves `antwanvdstap.com`.
5. Point the DNS for `antwanvdstap.com` and `www.antwanvdstap.com` to GitHub Pages.

## Push Commands

```bash
cd /home/antwan/antwanvanderstap.github.io
git init -b main
git add .
git commit -m "Initial personal website"
git remote add origin https://github.com/antwanvanderstap/antwanvanderstap.github.io.git
git push -u origin main
```

If you prefer SSH for pushing, use:

```bash
git remote add origin git@github.com:antwanvanderstap/antwanvanderstap.github.io.git
```
