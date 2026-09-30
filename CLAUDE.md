# corridorway-web — instructions for Claude sessions

WordPress site corridorway.com on cPanel. Custom block theme `corridorway-flagship`,
FormLayer forms, CookieAdmin/Complianz cookies. Local export was lost: the live
site is the source of truth.

## Start here
1. Check access: `WP_USER`, `WP_APP_PASSWORD`, `CPANEL_USER`, `CPANEL_API_TOKEN`,
   `CPANEL_HOST` env vars set, and `curl -I https://corridorway.com` works. If not,
   stop and tell the owner to set Network access (Custom: corridorway.com,
   *.corridorway.com, cPanel host) and the env vars in the cloud environment
   settings at claude.ai/code, then start a new session.
2. Full cPanel backup (files + DB) before anything else. Keep it out of git.
3. Staging: use host staging (WP Toolkit / Softaculous) or create
   staging.corridorway.com. Never edit production.
4. Pull `wp-content/themes/corridorway-flagship/` into the repo, commit as baseline.
5. Work `ACTION_REGISTER.md`: P1 first, group T and W, then E as evidence arrives.

## Audit pack
`audit/2026-09-29/` — REPORT.md, defect register, per-action prompts
(`02_ACTIONS_AND_PROMPTS/CWxx_*.md`), image slot sizes, design references.
The pack's MASTER_CHATGPT_PROMPT.txt rules apply to us too.

## Rules (from owner)
- Preserve approved logo, company name, identity and contact details.
- Never invent assays, grades, availability, licences, routes, mandates, case studies.
  Don't change >=90% gypsum to 98% without an approved assay.
- Real mineral, Berbera, office and operations photos only from approved originals;
  illustrative assets must not be presented as verified operating evidence.
- Status is lot-specific; use "sourcing opportunity / under qualification" until approved.
- Forms: no real submissions, suppress real notifications in staging.
- Don't edit core or plugin vendor files; use theme/templates/settings.
- Mark issues IMPLEMENTED NOT VERIFIED until retested at 320/375/390/768/1024/1440/1920.
- Never publish to production without explicit owner approval.
- Never commit credentials, wp-config.php, DB dumps or backups.

## Deliverables for owner review
Staging URL, before/after screenshots per issue, updated ACTION_REGISTER.md,
outstanding requirements list.
