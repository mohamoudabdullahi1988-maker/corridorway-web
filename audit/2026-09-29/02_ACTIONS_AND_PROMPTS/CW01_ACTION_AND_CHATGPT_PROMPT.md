# CW01 — Mineral availability
Priority: P1
Affected URL: https://corridorway.com/
Observed device: Chrome desktop 1363x936; other devices untested
Evidence: home.json; pages.json minerals; home.jpg (see 01_AUDIT_AND_EVIDENCE)

OBSERVED PROBLEM
Home calls gypsum, copper and gold Active; copper authority/assay/compliance pending and gold origin/authority/compliance pending in detailed passports.

BUSINESS CONSEQUENCE
Buyer may infer ready-to-offer supply.

READY ACTION
One approved data model; replace generic Active with inquiry/qualified statuses until lot gate met.

OWNER / ESTIMATE / DEPENDENCY
Trade lead + content + developer | 1-3 person-days | Current lot evidence approval

PASTE INTO CHATGPT WITH AFFECTED SOURCE AND SCREENSHOT
Implement CW01 for https://corridorway.com/ in the authorized source. Read this action card and the master prompt. Locate the real maintained template/component/plugin setting. Apply: One approved data model; replace generic Active with inquiry/qualified statuses until lot gate met.. Use the original screenshot for before evidence. Produce the actual edited source or patch, a preview and changed-file list. Keep unsupported business facts qualified. Do not publish. Validate: All home/detail badges agree; no active lot without approved authority, assay, specification and readiness.. Record tests actually run and leave untested checks open. Save exact after screenshots; do not label the proposal as a verified production fix.

ACCEPTANCE
All home/detail badges agree; no active lot without approved authority, assay, specification and readiness.

STATUS
PROPOSED — no production change verified. Capture before and after at the same viewport, record build ID, changed files, test/date and reviewer before marking CLOSED.
