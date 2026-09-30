# CW12 — Main landmark
Priority: P2
Affected URL: https://corridorway.com/company/
Observed device: Chrome desktop 1363x936; other devices untested
Evidence: home.json; details.json; minerals dedicated inspection (see 01_AUDIT_AND_EVIDENCE)

OBSERVED PROBLEM
No main or role=main landmark on all ten inspected pages.

BUSINESS CONSEQUENCE
Assistive navigation lacks main-content destination.

READY ACTION
Wrap unique body in one main with skip-link target.

OWNER / ESTIMATE / DEPENDENCY
Front-end + accessibility | 1 person-days | Template mapping

PASTE INTO CHATGPT WITH AFFECTED SOURCE AND SCREENSHOT
Implement CW12 for https://corridorway.com/company/ in the authorized source. Read this action card and the master prompt. Locate the real maintained template/component/plugin setting. Apply: Wrap unique body in one main with skip-link target.. Use the original screenshot for before evidence. Produce the actual edited source or patch, a preview and changed-file list. Keep unsupported business facts qualified. Do not publish. Validate: Exactly one main each page; skip link keyboard-visible and lands at content.. Record tests actually run and leave untested checks open. Save exact after screenshots; do not label the proposal as a verified production fix.

ACCEPTANCE
Exactly one main each page; skip link keyboard-visible and lands at content.

STATUS
PROPOSED — no production change verified. Capture before and after at the same viewport, record build ID, changed files, test/date and reviewer before marking CLOSED.
