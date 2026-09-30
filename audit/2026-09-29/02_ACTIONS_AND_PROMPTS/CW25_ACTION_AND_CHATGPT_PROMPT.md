# CW25 — Typography hierarchy
Priority: P2
Affected URL: https://corridorway.com/
Observed device: Chrome desktop 1363x936; other devices untested
Evidence: home.json headings (see 01_AUDIT_AND_EVIDENCE)

OBSERVED PROBLEM
Home service h5 compute 11px, mineral h4 12px versus 73.6px h1; heading-level jumps recur.

BUSINESS CONSEQUENCE
Compressed lower-page hierarchy and semantic inconsistency.

READY ACTION
Approved token scale; h3 for cards; persistent readable sizes and zoom QA.

OWNER / ESTIMATE / DEPENDENCY
Brand/UX + front-end | 1-3 person-days | Token approval

PASTE INTO CHATGPT WITH AFFECTED SOURCE AND SCREENSHOT
Implement CW25 for https://corridorway.com/ in the authorized source. Read this action card and the master prompt. Locate the real maintained template/component/plugin setting. Apply: Approved token scale; h3 for cards; persistent readable sizes and zoom QA.. Use the original screenshot for before evidence. Produce the actual edited source or patch, a preview and changed-file list. Keep unsupported business facts qualified. Do not publish. Validate: Repeat components share scale; no clipped text at requested widths/200% zoom; headings reflect nesting.. Record tests actually run and leave untested checks open. Save exact after screenshots; do not label the proposal as a verified production fix.

ACCEPTANCE
Repeat components share scale; no clipped text at requested widths/200% zoom; headings reflect nesting.

STATUS
PROPOSED — no production change verified. Capture before and after at the same viewport, record build ID, changed files, test/date and reviewer before marking CLOSED.
