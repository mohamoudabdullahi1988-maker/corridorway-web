# corridorway-web

Redesign of **corridorway.com** (WordPress on cPanel hosting).

The previous local export (`corridorway-export/`) was lost, so the live site is
the source of truth. Everything here is pulled from, and deployed back to, the
live server.

## Layout
- `BRIEF.md` — redesign goals, pages, tasks and status.
- `wp-content/themes/` — theme / child-theme code (added after first pull).
- `inventory/` — plugin list, page list, menus (added after first pull).

## Access (cloud sessions)
Set in the Claude Code cloud environment settings — never commit or paste in chat:

| Variable | What |
|---|---|
| `WP_USER`, `WP_APP_PASSWORD` | WordPress Application Password (Users → Profile) |
| `CPANEL_USER`, `CPANEL_API_TOKEN` | cPanel API token (Security → Manage API Tokens) |
| `CPANEL_HOST` | cPanel host, e.g. `server.example.com:2083` |

Network access must allow `corridorway.com` and the cPanel host.

## Rules
- Take a cPanel backup before any live change.
- Confirm each live change before applying it; prefer staging if the host offers it.
- Never commit credentials, `wp-config.php`, database dumps or backup archives.
