# CW13 — Buyer/supplier forms; also contact
Priority: P1
Affected URL: https://corridorway.com/trade/
Observed device: Chrome desktop 1363x936; other devices untested
Evidence: details.json fields; trade dedicated DOM/AX quoted in report (see 01_AUDIT_AND_EVIDENCE)

OBSERVED PROBLEM
Controls lack associated HTML labels/IDs; trade fields have no aria-label/labelledby; several AX controls unnamed.

BUSINESS CONSEQUENCE
Assistive users may not identify controls.

READY ACTION
Unique IDs per form/control, linked persistent label; name groups; accessible errors.

OWNER / ESTIMATE / DEPENDENCY
Front-end + form maintainer | 1-3 person-days | Form plugin/template ownership

PASTE INTO CHATGPT WITH AFFECTED SOURCE AND SCREENSHOT
Implement CW13 for https://corridorway.com/trade/ in the authorized source. Read this action card and the master prompt. Locate the real maintained template/component/plugin setting. Apply: Unique IDs per form/control, linked persistent label; name groups; accessible errors.. Use the original screenshot for before evidence. Produce the actual edited source or patch, a preview and changed-file list. Keep unsupported business facts qualified. Do not publish. Validate: Each field/checkbox announces correct name/required/state; native label click works; screen-reader and keyboard test passes.. Record tests actually run and leave untested checks open. Save exact after screenshots; do not label the proposal as a verified production fix.

ACCEPTANCE
Each field/checkbox announces correct name/required/state; native label click works; screen-reader and keyboard test passes.

STATUS
PROPOSED — no production change verified. Capture before and after at the same viewport, record build ID, changed files, test/date and reviewer before marking CLOSED.
