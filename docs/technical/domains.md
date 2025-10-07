# Domain Inventory

**Status:** active  
**Owner:** Austin Johnson  
**Last updated:** 2025-10-06  
**Next review:** 2025-11-01

| Domain | Purpose | Repo | Deployment Notes |
|--------|---------|------|------------------|
| austinbjohnson.com | Personal hub (this site) | `austinbjohnson/austinbjohnson.github.io` | CNAME committed; update Squarespace DNS (four GitHub A records + `www` CNAME) and toggle custom domain in Pages. |
| 28eme.ca | Consulting site (primary) | `austinbjohnson/28eme-site` | Live on GitHub Pages `main`; DNS pointed at GitHub IPs with HTTPS enforced. |
| 28eme.com | Consulting site (alias) | `austinbjohnson/28eme-site` | Squarespace domain forwarding -> `https://28eme.ca` (requires removing their default DNS before saving rule). |
| abj.lol | Personal micro-site / experiments | *(new repo TBD)* | Scaffold simple landing page; GitHub Pages deployment plan pending. |
| enseul.com | Creative project space | *(new repo TBD)* | Scaffold simple landing page; GitHub Pages deployment plan pending. |

Update this table whenever domains move or repos change. Detailed deployment steps live in `technical/deployment.md` and in each site repo.
