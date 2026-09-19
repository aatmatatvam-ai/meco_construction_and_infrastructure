# Meco Construction & Infratech — Website

Static, single-page website for Meco Construction & Infratech Private Limited (Manvi, Raichur district, Karnataka).

Plain HTML/CSS/JS — no build step, no framework, no dependencies to install.

## Structure

```
index.html        the entire site
assets/
  m-eranna.jpg     Managing Director photo
```

## Run it locally

Open `index.html` directly in a browser, or serve it so relative paths behave the same as in production:

```bash
python3 -m http.server 8000
# then open http://localhost:8000
```

## Before this goes live

A few things in the site are placeholders — search for `(sample)` in `index.html`:

- **Contact details** — email, phone, and the exact PIN code under "Contact" and "About"
- **CIN / registration number** — confirm the real Corporate Identification Number via the MCA portal and replace it in the "Company Data" panel
- **Project gallery** — the three cards under "Selected Work" are placeholder entries; swap in real completed/ongoing projects and photos
- **Quote form** — the contact form is a static UI only. It doesn't send anywhere yet. Wire it up to a form backend, e.g. [Formspree](https://formspree.io) or [Netlify Forms](https://docs.netlify.com/forms/setup/), or point it at an email/CRM endpoint.

## Hosting on GitHub Pages

Once this repo is pushed to GitHub:

1. Go to the repo's **Settings → Pages**
2. Under "Build and deployment", set **Source** to "Deploy from a branch"
3. Set **Branch** to `main` and folder to `/ (root)`
4. Save — GitHub will publish the site at `https://<your-username>.github.io/<repo-name>/`

No build step or GitHub Action is required since this is a plain static site.

### Custom domain (optional)

If you have a domain (e.g. `mecoconstruction.in`), add it under **Settings → Pages → Custom domain**, and point the domain's DNS at GitHub Pages per [GitHub's instructions](https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site).
