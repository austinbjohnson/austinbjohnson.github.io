# GitHub Pages Migration Plan

## Goal
Host a simple static website for 28eme using GitHub Pages and point the existing custom domain to it, keeping all services free.

## Repository
- GitHub repo: `https://github.com/austinbjohnson/somewhere`
- Preferred branch for the site: `main` (we can adjust if needed).

## Steps Overview
1. Enable GitHub Pages on the repo.
2. Add the static site files (start with a basic landing page).
3. Point the custom domain to GitHub Pages via DNS records.
4. Verify the live site and smooth out the update workflow.

## Step-by-Step

### 1. Enable GitHub Pages
- In GitHub, open `austinbjohnson/somewhere` → **Settings** → **Pages**.
- Under **Build and deployment**, choose **Source: Deploy from a branch**.
- Select branch `main` and folder `/ (root)` (or `/docs` if you prefer keeping the site in a subfolder).
- Save. GitHub assigns a temporary URL: `https://austinbjohnson.github.io/somewhere/`.

### 2. Add Site Files
- If the repo already has `index.html`, confirm it sits at the publish root you chose in Pages settings.
- If not, create a minimal `index.html` (we’ll draft it together next) and any supporting files like `/assets/styles.css`.
- Commit and push the changes via GitHub Desktop or the web editor.
- Wait ~1 minute for Pages to build; confirm the temp URL loads.

### 3. Add the Custom Domain
- Still in **Settings → Pages**, type your domain (e.g. `example.com`) into **Custom domain** and save.
- GitHub writes/updates a `CNAME` file at the publish root—keep this file committed.

### 4. Update DNS Records
- Sign into your domain registrar’s DNS control panel.
- For the apex/root domain (`example.com`): add four `A` records pointing to GitHub IPs:
  - `185.199.108.153`
  - `185.199.109.153`
  - `185.199.110.153`
  - `185.199.111.153`
- For `www.example.com`: add a `CNAME` record pointing to `austinbjohnson.github.io`.
- Remove old Squarespace DNS entries so only the GitHub ones remain.
- Save and wait for DNS to propagate (can take up to a few hours).

### 5. Verify & Maintain
- After DNS resolves, visit `https://example.com` and `https://www.example.com` to confirm the site loads.
- In GitHub Pages settings, ensure **Enforce HTTPS** is checked (it appears once GitHub detects the domain).
- For future edits: modify files locally, commit, and push; GitHub redeploys automatically.

## Optional Enhancements
- Use a free HTML template (Start Bootstrap, HTML5 UP, etc.) to improve the design quickly.
- Hook up a contact form via Formspree or Netlify Forms (free tiers available).
- Consider Cloudflare (free) only if you want DNS management extras; not required for basic hosting.

---
Ready for the next step? Let me know and we’ll draft the starter `index.html` together or walk through the GitHub Pages toggle live.
