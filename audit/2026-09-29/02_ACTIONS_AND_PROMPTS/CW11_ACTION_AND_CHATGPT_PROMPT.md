# CW11 — Duplicate portfolio
Priority: P2
Affected URL: https://corridorway.com/minerals/
Observed device: Chrome desktop 1363x936; other devices untested
Evidence: pages.json; minerals.jpg (see 01_AUDIT_AND_EVIDENCE)

OBSERVED PROBLEM
Gypsum/copper/gold have summary plus repeated full descriptions/passports.

BUSINESS CONSEQUENCE
Status drift and excessive reading length.

READY ACTION
One canonical detail per mineral; summaries use shared record.

OWNER / ESTIMATE / DEPENDENCY
UX + developer | 2-4 person-days | Approved content model

PASTE INTO CHATGPT WITH AFFECTED SOURCE AND SCREENSHOT
Implement CW11 for https://corridorway.com/minerals/ in the authorized source. Read this action card and the master prompt. Locate the real maintained template/component/plugin setting. Apply: One canonical detail per mineral; summaries use shared record.. Use the original screenshot for before evidence. Produce the actual edited source or patch, a preview and changed-file list. Keep unsupported business facts qualified. Do not publish. Validate: One master record per material; compact summaries link correct section; no contradictory duplicates.. Record tests actually run and leave untested checks open. Save exact after screenshots; do not label the proposal as a verified production fix.

ACCEPTANCE
One master record per material; compact summaries link correct section; no contradictory duplicates.

STATUS
PROPOSED — no production change verified. Capture before and after at the same viewport, record build ID, changed files, test/date and reviewer before marking CLOSED.
