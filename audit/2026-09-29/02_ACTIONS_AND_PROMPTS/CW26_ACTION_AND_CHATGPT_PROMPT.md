# CW26 — Media delivery
Priority: P2
Affected URL: https://corridorway.com/
Observed device: Chrome desktop 1363x936; other devices untested
Evidence: home.json and details.json images (see 01_AUDIT_AND_EVIDENCE)

OBSERVED PROBLEM
Most important raw images lack srcset; inner images often loading auto. No payload/CWV measurements.

BUSINESS CONSEQUENCE
Potential excess transfer; performance effect not measured.

READY ACTION
Measure then responsive renditions/lazy loading/reserved dimensions; prioritize actual LCP.

OWNER / ESTIMATE / DEPENDENCY
Performance + front-end | 2-4 person-days | PSI/Lighthouse and asset provenance

PASTE INTO CHATGPT WITH AFFECTED SOURCE AND SCREENSHOT
Implement CW26 for https://corridorway.com/ in the authorized source. Read this action card and the master prompt. Locate the real maintained template/component/plugin setting. Apply: Measure then responsive renditions/lazy loading/reserved dimensions; prioritize actual LCP.. Use the original screenshot for before evidence. Produce the actual edited source or patch, a preview and changed-file list. Keep unsupported business facts qualified. Do not publish. Validate: Appropriate source at widths/DPR; dimensions reserved; before/after actual measurements attached; no unsupported speed claims.. Record tests actually run and leave untested checks open. Save exact after screenshots; do not label the proposal as a verified production fix.

ACCEPTANCE
Appropriate source at widths/DPR; dimensions reserved; before/after actual measurements attached; no unsupported speed claims.

STATUS
PROPOSED — no production change verified. Capture before and after at the same viewport, record build ID, changed files, test/date and reviewer before marking CLOSED.
