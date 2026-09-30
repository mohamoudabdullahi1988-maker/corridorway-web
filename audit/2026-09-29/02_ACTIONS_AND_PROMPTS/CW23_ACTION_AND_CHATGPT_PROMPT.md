# CW23 — Legal headings; also terms
Priority: P2
Affected URL: https://corridorway.com/privacy/
Observed device: Chrome desktop 1363x936; other devices untested
Evidence: details.json legal; terms.jpg (see 01_AUDIT_AND_EVIDENCE)

OBSERVED PROBLEM
Two h1 headings repeat Privacy Policy and Terms of Use.

BUSINESS CONSEQUENCE
Duplicated title and hierarchy.

READY ACTION
Render one h1 each, retain h2 subsection structure.

OWNER / ESTIMATE / DEPENDENCY
Front-end/editor | 0.25 person-days | Template/title mapping

PASTE INTO CHATGPT WITH AFFECTED SOURCE AND SCREENSHOT
Implement CW23 for https://corridorway.com/privacy/ in the authorized source. Read this action card and the master prompt. Locate the real maintained template/component/plugin setting. Apply: Render one h1 each, retain h2 subsection structure.. Use the original screenshot for before evidence. Produce the actual edited source or patch, a preview and changed-file list. Keep unsupported business facts qualified. Do not publish. Validate: One visible primary title per legal page; no duplicate heading in DOM/AX.. Record tests actually run and leave untested checks open. Save exact after screenshots; do not label the proposal as a verified production fix.

ACCEPTANCE
One visible primary title per legal page; no duplicate heading in DOM/AX.

STATUS
PROPOSED — no production change verified. Capture before and after at the same viewport, record build ID, changed files, test/date and reviewer before marking CLOSED.
