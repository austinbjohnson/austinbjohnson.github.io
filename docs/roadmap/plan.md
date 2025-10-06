# Web Presence Roadmap

**Status:** active  
**Owner:** Austin Johnson  
**Last updated:** 2025-02-14  
**Next review:** 2025-03-15

## Goals
1. Serve `austinbjohnson.com` as the personal hub (bio, hobbies, writing).
2. Launch `28eme.ca` as the consulting and automation portfolio.
3. Keep both hosting stacks free via GitHub Pages.

## Repositories
- Personal site: `https://github.com/austinbjohnson/austinbjohnson.github.io`
- Consulting site: `https://github.com/austinbjohnson/28eme-site` *(to be created)*

## Milestones
1. ✅ Personal site foundation and initial copy.
2. 🔄 Establish docs workflow (`docs/` hierarchy) for planning.
3. ☐ Bootstrap `28eme-site` repo and draft service-oriented homepage.
4. ☐ Configure custom domains and DNS for both sites.
5. ☐ Publish hobby subpages after content outlines are ready.

## Deployment Checklist (per site)
1. Confirm repo is public.
2. Settings → Pages → “Deploy from a branch” (`main` + `/`).
3. Add `CNAME` file automatically via Pages settings; commit it.
4. Update registrar DNS records (four `A` records + `www` `CNAME`).
5. Verify HTTPS and note go-live date in `docs/changelog.md`.

## Backlog Ideas
- Draft lightweight design system shared between sites.
- Add GitHub Action to lint HTML/CSS prior to deploy.
- Create contact form using Formspree or similar service.
- Explore analytics (Plausible, Simple Analytics) if needed.

Keep this document updated as milestones shift. Archive completed initiatives in `docs/changelog.md`.
