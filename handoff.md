# Handoff Reference

This repo follows the shared workflow documented at the websites root.

- Master session notes: `../handoff/SESSION_NOTES.md`
- Co-dev reminders: `../REMINDER.md`

## Site-Specific Notes

- [ ] Confirm `www.austinbjohnson.com` serves the GitHub Pages build over HTTPS and update docs once the alias resolves. (2025-10-07 04:11 UTC: still serves Squarespace 404.)
- [ ] Investigate the Firefox redirect loop (likely leftover Squarespace redirect vs. apex records) and document the fix. Initial check shows apex `austinbjohnson.com` 301s to `https://www.austinbjohnson.com/`, which is still pointed at Squarespace.
- [x] Simplify the homepage content footprint (contact CTA removed; Strava/Goodreads placeholders added along with Now/reading/automation module roadmap).
