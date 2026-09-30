# corridorway.com redesign — brief

Status: **setup** · Started 2026-09-30

## Goals
_To fill in with owner: what the redesign should achieve (look, audience, conversions)._

## Platform
- WordPress on cPanel hosting (keep current platform).
- Page builder: _unknown — check on first pull._

## Phase 0 — access and backup
- [ ] Allow `corridorway.com` + cPanel host in environment network access
- [ ] Add `WP_*` / `CPANEL_*` environment variables
- [ ] Full cPanel backup (files + database), stored off the repo
- [ ] Pull theme files into `wp-content/themes/`
- [ ] Inventory: plugins, pages, menus, media count → `inventory/`

## Phase 1 — audit
- [ ] Current page list and navigation
- [ ] Mobile layout, speed, broken links
- [ ] WordPress / plugin / PHP versions and updates

## Phase 2 — redesign
- [ ] Agree design direction (colours, fonts, layout)
- [ ] Child theme changes
- [ ] Page-by-page content and layout updates

## Phase 3 — launch
- [ ] Final review with owner
- [ ] Deploy, verify, post-launch backup

## Decisions log
- 2026-09-30: New private repo `corridorway-web`; live site is source of truth
  (local export lost); work runs from Claude Code cloud sessions.
