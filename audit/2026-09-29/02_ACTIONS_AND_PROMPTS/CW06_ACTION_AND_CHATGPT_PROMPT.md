# CW06 — Shared footer
Priority: P2
Affected URL: https://corridorway.com/
Observed device: Chrome desktop 1363x936; other devices untested
Evidence: home.json links + pages.json IDs (see 01_AUDIT_AND_EVIDENCE)

OBSERVED PROBLEM
11 fragment links target absent IDs on gateway, responsible-trade and intelligence.

BUSINESS CONSEQUENCE
Footer navigation fails promised destination.

READY ACTION
Remove unsupported targets or connect to existing real sections; do not insert empty sections.

OWNER / ESTIMATE / DEPENDENCY
Front-end + editor | 1 person-days | Information architecture approval

PASTE INTO CHATGPT WITH AFFECTED SOURCE AND SCREENSHOT
Implement CW06 for https://corridorway.com/ in the authorized source. Read this action card and the master prompt. Locate the real maintained template/component/plugin setting. Apply: Remove unsupported targets or connect to existing real sections; do not insert empty sections.. Use the original screenshot for before evidence. Produce the actual edited source or patch, a preview and changed-file list. Keep unsupported business facts qualified. Do not publish. Validate: All 11 fragments locate intended nonempty sections or links removed; all-page regression passes.. Record tests actually run and leave untested checks open. Save exact after screenshots; do not label the proposal as a verified production fix.

ACCEPTANCE
All 11 fragments locate intended nonempty sections or links removed; all-page regression passes.

STATUS
PROPOSED — no production change verified. Capture before and after at the same viewport, record build ID, changed files, test/date and reviewer before marking CLOSED.
