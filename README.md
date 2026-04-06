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
5. Add `antwanvdstap.com` as the custom domain in `Settings -> Pages`.
6. Verify the domain in your GitHub account `Settings -> Pages` to reduce takeover risk.
7. Point the DNS for `antwanvdstap.com` and `www.antwanvdstap.com` to GitHub Pages.

## DNS Records

For the apex domain `antwanvdstap.com`, GitHub Pages supports either:

- `A` records for `@` pointing to `185.199.108.153`
- `A` records for `@` pointing to `185.199.109.153`
- `A` records for `@` pointing to `185.199.110.153`
- `A` records for `@` pointing to `185.199.111.153`
- Optional `AAAA` records for `@` pointing to `2606:50c0:8000::153`
- Optional `AAAA` records for `@` pointing to `2606:50c0:8001::153`
- Optional `AAAA` records for `@` pointing to `2606:50c0:8002::153`
- Optional `AAAA` records for `@` pointing to `2606:50c0:8003::153`

For `www.antwanvdstap.com`, create:

- `CNAME` record for `www` pointing to `antwanvanderstap.github.io`

Avoid wildcard DNS records such as `*.antwanvdstap.com`.

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
