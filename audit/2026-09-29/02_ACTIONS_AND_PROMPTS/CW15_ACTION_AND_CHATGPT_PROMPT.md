# CW15 — Form privacy notice; also contact
Priority: P2
Affected URL: https://corridorway.com/trade/
Observed device: Chrome desktop 1363x936; other devices untested
Evidence: Trade DOM privacyLinks=[]; details.json (see 01_AUDIT_AND_EVIDENCE)

OBSERVED PROBLEM
Privacy/Terms consent wording is plain text; trade form has no anchors to policies.

BUSINESS CONSEQUENCE
User cannot inspect referenced notices beside submission.

READY ACTION
Link notices, distinguish inquiry processing from optional marketing; review actual basis.

OWNER / ESTIMATE / DEPENDENCY
Form developer + privacy reviewer | 0.5-1 person-days | Approved privacy content

PASTE INTO CHATGPT WITH AFFECTED SOURCE AND SCREENSHOT
Implement CW15 for https://corridorway.com/trade/ in the authorized source. Read this action card and the master prompt. Locate the real maintained template/component/plugin setting. Apply: Link notices, distinguish inquiry processing from optional marketing; review actual basis.. Use the original screenshot for before evidence. Produce the actual edited source or patch, a preview and changed-file list. Keep unsupported business facts qualified. Do not publish. Validate: Notices keyboard accessible adjacent to submit; optional marketing separate and unchecked.. Record tests actually run and leave untested checks open. Save exact after screenshots; do not label the proposal as a verified production fix.

ACCEPTANCE
Notices keyboard accessible adjacent to submit; optional marketing separate and unchecked.

STATUS
PROPOSED — no production change verified. Capture before and after at the same viewport, record build ID, changed files, test/date and reviewer before marking CLOSED.
