# Deployment & DNS Reference

**Status:** draft  
**Owner:** Austin Johnson  
**Last updated:** 2025-02-14  
**Next review:** 2025-03-01

## Personal Site (`austinbjohnson.com`)
- Repo: `austinbjohnson/austinbjohnson.github.io`
- GitHub Pages: branch `main`, directory `/`.
- DNS: apex `A` records → `185.199.108.153`, `185.199.109.153`, `185.199.110.153`, `185.199.111.153`; `www` `CNAME` → `austinbjohnson.github.io`.
- HTTPS: enable “Enforce HTTPS” after DNS propagates.

## Consulting Site (`28eme.ca`)
- Repo: `austinbjohnson/28eme-site` (to be created).
- GitHub Pages: plan to deploy from `main` branch.
- DNS: mirror the same `A` records for apex and point `www` `CNAME` → `austinbjohnson.github.io` or the repo-specific Pages domain once live.

## Workflow Notes
1. Commit changes to `main`; GitHub Pages rebuilds automatically (allow ~1 minute).
2. When editing DNS, remove legacy Squarespace entries before adding GitHub records.
3. After any DNS change, verify both apex and `www` respond over HTTPS.
4. Document significant infrastructure changes in `docs/changelog.md`.

## Future Improvements
- Automate checks with a simple script (curl + status) to confirm Pages deployment success.
- Draft a GitHub Action that validates HTML accessibility before deploy.
