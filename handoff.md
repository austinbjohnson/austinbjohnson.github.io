# Handoff Reference

This repo follows the shared workflow documented at the websites root.

- Master session notes: `../handoff/SESSION_NOTES.md`
- Co-dev reminders: `../REMINDER.md`

## Site-Specific Notes

- [ ] Confirm `www.austinbjohnson.com` serves the GitHub Pages build over HTTPS and update docs once the alias resolves. (2025-10-07 04:31 UTC: still serves Squarespace 404.)
- [ ] Investigate the Firefox redirect loop (likely leftover Squarespace redirect vs. apex records) and document the fix. Apex `austinbjohnson.com` continues to 301 toward the Squarespace-backed `www` host.
- [x] Simplify the homepage content footprint (contact CTA removed; Strava/Goodreads placeholders added along with Now/reading/automation module roadmap). Merged via PR #2 into `feat/custom-domain`.
- [ ] Hook the telemetry placeholders to live Strava/Goodreads data once automation endpoints or feeds are available.
