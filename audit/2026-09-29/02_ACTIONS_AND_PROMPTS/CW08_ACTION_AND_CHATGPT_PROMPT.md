# CW08 — Download Product Sheet
Priority: P2
Affected URL: https://corridorway.com/minerals/
Observed device: Chrome desktop 1363x936; other devices untested
Evidence: Mineral DOM inspection quoted in report D; minerals.jpg (see 01_AUDIT_AND_EVIDENCE)

OBSERVED PROBLEM
Download label href is trade#buyer-requirement.

BUSINESS CONSEQUENCE
Expected download not delivered.

READY ACTION
Provide approved actual product sheet or rename Request product sheet.

OWNER / ESTIMATE / DEPENDENCY
Trade lead + developer | 0.5-2 person-days | Approved product sheet if download retained

PASTE INTO CHATGPT WITH AFFECTED SOURCE AND SCREENSHOT
Implement CW08 for https://corridorway.com/minerals/ in the authorized source. Read this action card and the master prompt. Locate the real maintained template/component/plugin setting. Apply: Provide approved actual product sheet or rename Request product sheet.. Use the original screenshot for before evidence. Produce the actual edited source or patch, a preview and changed-file list. Keep unsupported business facts qualified. Do not publish. Validate: Label and action agree; real file opens/downloads or clearly labeled request reaches inquiry.. Record tests actually run and leave untested checks open. Save exact after screenshots; do not label the proposal as a verified production fix.

ACCEPTANCE
Label and action agree; real file opens/downloads or clearly labeled request reaches inquiry.

STATUS
PROPOSED — no production change verified. Capture before and after at the same viewport, record build ID, changed files, test/date and reviewer before marking CLOSED.
