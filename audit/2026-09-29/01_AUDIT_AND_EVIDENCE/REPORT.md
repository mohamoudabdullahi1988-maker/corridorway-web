# Corridorway — Live Website Audit & Transformation Brief

**Audit date:** 29 September 2026 (Africa/Nairobi). **Website:** https://corridorway.com/.
**Decision:** Stabilize credibility, navigation and inquiry accessibility before investing in a wholesale redesign. No production changes were made, and no inquiry was submitted.

## A. Executive findings and coverage

The most consequential defect is inconsistent commercial status. The homepage labels gypsum, copper and gold availability active. Copper's detailed passport has selling authority, assay and compliance pending; gold has origin, selling authority and compliance pending and assay not published. This is an internal contradiction, not a determination that the company lacks private supporting documents.

The homepage also presents origin, ownership, assay, specification, payment terms and logistics as completed checks without identifying a lot, record, reviewer or date. Its evidence link leads to a general commitment page. The mineral page publishes specific gypsum chemistry and year-round supply claims without an identifiable supporting report in the inspected content. These claims need company evidence approval rather than stronger promotional language.

The inquiry routes exist and the buyer anchor reaches its form. However, the form controls inspected lack associated HTML labels, IDs and ARIA labels; several appear unnamed in the browser accessibility tree. The product-sheet download actually leads to the buyer form. Eleven shared footer fragment destinations are absent from their destination pages. Social icons point to the current page's `#`.

The existing navy/gold identity and two primary buyer/supplier paths should be retained. The improvements should make proof explicit, labels accurate, forms accessible and components consistent.

### What was actually tested

| Area | Coverage | Evidence/limit |
|---|---|---|
| Public pages | 10 rendered pages: homepage, seven core internal pages and two legal pages | Navigation/footer discovery; browser DOM/text and titles; screenshots in evidence/ |
| Desktop browser | Cloud Chrome, reported inner viewport 1363 × 936 CSS px | No OS/version identification or other browser tests |
| Visual evidence | Full-page desktop screenshots saved for all 10 pages | Detailed visual review of home/minerals top, buyer anchor, company/contact/gateway/responsible/intelligence and terms; privacy and lower home/minerals/trade screenshot inspection less complete |
| Page semantics | DOM headings, landmarks, canonical tags, images and fields on inspected pages | No automated axe scan; no screen reader session |
| Interaction | Reject All cookie choice; company submenu expansion; buyer deep link; mineral assay panel via its visible label; catalog search for Tantalum | These worked in the observed desktop state; other interactions remain untested |
| Internal destinations | Main paths rendered; fragment IDs checked against destination DOM | Not a status-code crawler; not all external links clicked |
| Forms | Fields, visible copy, HTML method and labels inspected | Submission, validation, backend routing and receipt NOT TESTED |
| Benchmark research | Current official Trafigura, Glencore, IXM content/navigation retrieved | Benchmark responsive behavior, performance and visual rendering NOT TESTED |
| robots/sitemap | Search retrieval failed for both; robots browser navigation blocked by client policy | Not evidence of site outage or missing files; sitemap browser inspection NOT TESTED; no bypass attempted |
| Mobile / other sizes | NOT TESTED | Browser API exposed no viewport-resize control; requested 375/390/768/1024/1440/1920 matrix remains open |
| Performance/security | NOT TESTED except HTTPS rendered and public privacy/cookie UI observed | No Lighthouse, PSI, CrUX, response headers, traffic capture, TLS configuration, server or analytics access |

This is a substantive **desktop/public-content audit with a developer handoff**, not a completed all-device certification. Sitemap discovery and authenticated technical tests remain prerequisites to a comprehensive final score. Public page rendering is not an HTTP 200 measurement. The preliminary terminal HTTP request failed because the execution proxy was unavailable; it yielded no website headers.

## B. Discovered URL inventory

All rows below rendered in Chrome. Titles and final trailing-slash URLs came from the live browser. Section counts are editorial body modules, excluding shared header/footer; they are not counts of every DOM container.

| URL | Page title | Function / audience | Major sections | Principal CTA | Main issue IDs |
|---|---|---|---:|---|---|
| https://corridorway.com/ | Corridorway – Mineral trade intelligence, verification and Berbera-connected market access. | Positioning; buyers, suppliers, partners | 10 | Submit a buyer requirement | CW01,02,06,07,14 |
| https://corridorway.com/company/ | Company – Corridorway | Identity, approach, governance; all counterparties | 5 | Email / phone | CW03,09,12 |
| https://corridorway.com/minerals/ | Minerals – Corridorway | Portfolio and regional potential; buyers | 10 | I am a buyer | CW01,04,05,08,10,11 |
| https://corridorway.com/trade/ | Trade – Corridorway | Services; separate buyer and supplier forms | 5 | Submit Buyer Requirement / Supply Opportunity | CW13,15,16 |
| https://corridorway.com/berbera-gateway/ | Berbera Gateway – Corridorway | Logistics positioning; buyers/logistics partners | 4 | Explore Route Intelligence | CW06,17,18 |
| https://corridorway.com/responsible-trade/ | Responsible Trade – Corridorway | Responsible sourcing process; institutional buyers | 3 | Learn Our Approach | CW06,09,19 |
| https://corridorway.com/intelligence/ | Trade Intelligence – Corridorway | Intended market briefs; buyers | 3 | None in body | CW06,07,09,20 |
| https://corridorway.com/contact/ | Contact – Corridorway | Inquiry, email/phone/WhatsApp; all audiences | 3 | Send Message | CW09,13,15,21 |
| https://corridorway.com/privacy/ | Privacy Policy – Corridorway | Data notice; visitors/inquirers | 4 | Footer contacts | CW22,23 |
| https://corridorway.com/terms/ | Terms of Use – Corridorway | General use conditions; visitors | 4 | Footer contacts | CW23 |

Additional discovered technical URLs: `/feed/`, `/comments/feed/`, public WordPress API/oEmbed links and asset paths in homepage metadata. They were not crawled and are not treated as additional marketing pages. No live article-detail pages were discovered through the inspected navigation. The lack of sitemap access means the inventory cannot be certified exhaustive.

### Fragment inventory

Present: company `approach`, `governance`, `contact`; minerals `gypsum`, `copper`, `gold`, `expanded-catalog` and radio-panel IDs; trade `buyer-requirement`, `supply-opportunity`.

Absent in inspected destination DOM: gateway `logistics`, `connectivity`, `routes`; responsible-trade `commitment`, `policies`, `standards`, `evidence`; intelligence `markets`, `logistics`, `minerals`, `reports`. These 11 links are navigation defects even though their parent pages render. Do not create empty sections simply to satisfy links: remove unsupported links or connect to real content.

## C. Brand and design system

Observed: display headings compute to `Inter Tight, Inter, system-ui, sans-serif`; homepage h1 is 73.6px at the observed viewport. Process labels use the proposed gold `rgb(210,173,98)` and movement uses copper `rgb(200,117,66)`. These are computed CSS observations, not proof every font downloaded or all palette tokens were deployed. Licensing was not audited. Homepage mineral names are 12px, trade-service headings 11px, main section headings approximately 20.445px and closing CTA 28px. The hierarchy feels compressed below a very large hero (professional judgment).

The logo uses the same source family in header and footer at about 160×40 and 170×43. The identity geometry has not been compared against an approved master. Source uses responsive WordPress derivatives. Preserve the master, approved proportions and naming. Specify a proposed clear space of half the symbol height, subject to brand-owner approval; do not redraw it.

### Proposed canonical tokens — approval reference, not deployed code

| Token | Value | Role |
|---|---|---|
| abyss-navy | #061522 | Main dark canvas |
| atlantic-navy | #0B2237 | Alternate sections/header |
| deep-slate | #1B2B38 | Cards |
| mineral-ivory | #F4F1EA | Light editorial canvas |
| white | #FFFFFF | Dark-canvas text |
| mist | #E7ECEF | Light dividers/surfaces |
| signal-gold | #D2AD62 | Primary action, emphasis |
| copper-pulse | #C87542 | Selective process emphasis |
| intelligence-blue | #4D7CFE | Intelligence accents, subject to contrast testing |
| verification-teal | #18A999 | Status accents, never sole status indicator |
| graphite | #171D22 | Light-canvas text |

Use Inter Tight for h1–h3 and Inter for body/UI. Load only required weights, self-host WOFF2 where authorized and set `font-display:swap`. Use IBM Plex Mono only for lot IDs, assays and small technical labels. Defer Newsreader unless a real editorial series needs it. Font-family declarations do not establish license status.

| Component | Exact proposed specification |
|---|---|
| Spacing scale | 4, 8, 12, 16, 24, 32, 48, 64, 96px; no arbitrary repeated-component offsets |
| Container | max-width 1280px; centered; side padding 20px mobile, 32px tablet, 48px desktop |
| Grid | 4 mobile, 8 tablet, 12 desktop tracks; 24px desktop / 16px mobile gap |
| Type | body 16px/1.6; lead 20px/1.5; small 14px/1.5; technical 12px/1.5; h1 clamp(36px,5vw,72px)/1.05; h2 clamp(28px,3vw,40px)/1.15; h3 22px/1.3 |
| Section rhythm | 48px mobile, 64px tablet, 96px desktop block padding; compact utility modules may use 32px |
| Buttons | min-height 48px; padding 12px 20px; radius 6px; 16px/1.25 Inter 600; gold/graphite primary; explicit hover/focus/disabled states |
| Cards | radius 8px; padding 24px; same sibling media ratio and gap; no hard fixed text height |
| Forms | control 48px minimum; 16px text; visible label above; 8px label gap; 24px field gap; max form width 720px |
| Icons | One licensed vector family, 24px, consistent 1.5–2px stroke; decorative `aria-hidden`; named buttons |
| Focus | 3px high-contrast outline plus 3px offset; test on both dark and light backgrounds |
| Shadows | none by default; floating menu `0 8px 24px rgba(6,21,34,.18)` |
| Breakpoints | 640px, 768px, 1024px, 1280px; header collapses based on measured fit, initially ≤1024px |

Do not use teal, copper or blue indiscriminately for small text on ivory. Required measured contrast: normal text ≥4.5:1, large text ≥3:1; applicable UI boundaries/state indicators ≥3:1. No live contrast pass is claimed. Token proposals require contrast checks before approval.

## D. Page and section change specification

The rows below follow body reading order. Shared header/footer changes apply everywhere. PURPOSE states buyer utility; ACTION is a recommendation. Visual judgments are distinguished from content/DOM facts.

| Page / section | Purpose and observed issue | Action / exact change |
|---|---|---|
| Home / hero | Brand slogan, buyer and supply CTAs; business scope only in supporting line | KEEP slogan; REFINE lead to explicitly name Corridorway's sourcing and qualification role after capability approval; retain two distinct CTAs; authenticate port image |
| Home / process | Four stage model; copy implies all sources already verified | REFINE to describe checks performed at each stage rather than universal completed status; use h2 plus h3 |
| Home / minerals | Three active labels conflict with detailed passports | REPLACE badges with approved statuses drawn from one source; lot-specific evidence only |
| Home / gateway | Berbera positioning and map | REFINE diagram caption and link to documented logistics page; preserve enough space for readable labels |
| Home / evidence | Unscoped completed checks | REPLACE with 'Checks before an offer'; explain method, not completed transaction; link to documented criteria |
| Home / services | Six very small headings | REFINE h3 to 22px; concise benefit per service; use common cards; align services with trade page |
| Home / intelligence | Three Read more links but briefs coming soon | REMOVE Read more until individual article exists; MERGE into a single honest preparation notice or publish a sourced brief |
| Home / responsible trade | Laboratory visual and framework commitments | REFINE to process and approved records; label illustrative imagery where applicable |
| Home / closing CTA | Buyer/supply selection | KEEP; labels match destination; no unsupported 'global partners' implication |
| Home / shared footer | Dense seven-column arrangement; broken fragments and placeholders | REFINE links and reduce columns at intermediate widths; retain visible contact details |
| Company / hero | 'Sovereign' can imply governmental mandate; image describes actual company building | REPLACE 'sovereign' unless documented mandate; proposed 'A minerals trade office based in Berbera, Somaliland.' Authenticate or label image |
| Company / About | Operational capability statement | REFINE to approved scope and exact legal entity; avoid assuming offices/assets owned |
| Company / Approach | Every listing said to carry evidence passport | KEEP method but define statuses, approval gates and last-review date |
| Company / Governance | Legal and chain-of-custody assertions | REFINE against registration/licensing and documented process; publish approved factual disclosures |
| Company / Contact | Correct public contact strings | KEEP; canonical Contact route in shared navigation |
| Minerals / hero | Broad verified/high-quality language | REFINE to distinguish inquiry-led sourcing from verified lots |
| Minerals / category overview | Three audience/product families | KEEP; make navigation destinations explicit and consistent |
| Minerals / featured gypsum | Chemistry and supply readiness without named lab/lot | REFINE or withhold commercial specification pending approved assay; add moisture/dry basis, sampling method and lot context |
| Minerals / tab panels | Assay panel shows statuses only; visible label interaction worked | REFINE with dated evidence summary; implement accessible disclosure/tab behavior and keyboard testing; product sheet must match label |
| Minerals / portfolio | Copper and gold cards precede duplicate long profiles | MERGE each product into one canonical section; card summaries can link to it |
| Minerals / mid-page CTA | Appears before repeated detailed sections | REORDER after coherent portfolio or use compact inline CTA |
| Minerals / gypsum detail | Repeats feature and evidence status | MERGE with featured gypsum; one source of truth |
| Minerals / copper detail | 'Cathode-grade concentrate' mixes product forms; assay pending | REPLACE with form accurately supported by assay; otherwise 'Copper sourcing opportunity — specification subject to qualification' |
| Minerals / gold detail | Verified-source prose versus origin pending | REFINE to controlled inquiry opportunity; no offer until authority, origin, assay and compliance approved |
| Minerals / expanded catalog | Clear caveats but includes editorial commands to site author | KEEP opportunity/potential separation; REPLACE instructions with buyer copy; link precise regional-source documents; search for Tantalum worked |
| Trade / hero | General service promise | KEEP with authenticated or clearly illustrative vessel image |
| Trade / raster workflow | Large 1300×726 rendered workflow graphic | REPLACE with semantic HTML ordered list; avoid raster text and duplicate process explanation |
| Trade / service grid | Nine services; h5 labels under h2 | REFINE h3 hierarchy and shared spacing; justify differences from home |
| Trade / buyer form | Serious buying inputs exist; delivery basis absent; no linked policy in form | REFINE fields and labels as section H; staging-only delivery test |
| Trade / supplier form | Useful origin/authority inputs | REFINE labels, safe disclosure guidance, routing and review acknowledgement |
| Gateway / hero | Port scale/location | KEEP position; authenticate image; avoid implying owned infrastructure |
| Gateway / advantages | 18m+ depth and efficiency assertions unsourced in content | REFINE using dated terminal/operator documentation; distinguish depth from permitted vessel draft |
| Gateway / routes | Map and transit bands all Active; CTA reaches coming-soon page | REFINE named ports/service/routing/date basis; mark indicative; route inquiry CTA to contact instead of empty intelligence |
| Gateway / logistics chain | Three stages of movement | KEEP; list responsibility handoffs, documentation and quote-dependent transit |
| Responsible / hero | Image laboratory but alt says quarry | REFINE matching alt and authentic/illustrative labeling |
| Responsible / two evidence illustrations | Field camp and assay papers | REFINE caption and provenance; these are not operational evidence |
| Responsible / six commitments | OECD, community, HSE and owner/source claims | REFINE to approved policies with owners/versions; publish only actual procedures; one method CTA |
| Intelligence / hero | Port aerial image alt says professionals reviewing reports | REFINE matching alt; purposeful editorial image |
| Intelligence / three cards | All coming soon; different media ratios create uneven card height | MERGE honest empty state until ready; then standard 16:9 media, date, author, source, unique detail URL |
| Intelligence / source statement | Sensible publication gate | KEEP; actually require source approval in editorial workflow |
| Contact / hero | Visibly soft port crop with stray embedded text at left | REPLACE authenticated clean source; avoid baked-in text, check focus/crop |
| Contact / contacts + message | Correct contact strings; form dominates height, with sparse left column | KEEP direct contacts; REFINE compact field layout and accessible labels; phone/email app launch not tested |
| Contact / visit | Directions searches Berbera Port rather than a confirmed office | REFINE label to 'View Berbera area' until exact visitor location approved; do not infer port access permission |
| Privacy / title and notice | Two h1s; short general notice | MERGE duplicate heading; REFINE actual processing, cookie details, retention and request channel after qualified review |
| Terms / title and conditions | Two h1s; general disclaimer | MERGE duplicate heading; retain company-approved conditions; no legal sufficiency opinion given |

## E. Images and media

The companion `image-manifest.csv` inventories important HTML image occurrences by source URL, page, alt text, reported natural dimensions, rendered dimensions, ratio, loading and srcset. CSS background-only assets, payload bytes, EXIF and ownership were not fully inventoried. Browser `naturalWidth` can be density-corrected when srcset is used; it is not always an independently decoded file-pixel measurement. All format labels are filename extensions, not verified Content-Type.

Observed assets include 1024×1024 mineral JPEGs reused at small homepage and larger mineral sizes; most raw images have no srcset. Homepage hero is reported 1376×768, eagerly loaded, without srcset; many inner-page images are loading=auto. Some pages have responsive WordPress derivatives. Absence of srcset is a delivery opportunity, not proof of a measured Core Web Vitals failure. No claim of stretched images is made solely from differing rendered ratios: object-fit/crop must be checked.

| Replacement group | Evidence / priority | Production brief and acceptance |
|---|---|---|
| Company hero `Gemini_Generated_Image_hq33alhq33alhq33.png` | P1; alt describes actual Corridorway building; filename indicates generated-image origin but provenance not proven | Authenticate ownership/location or clearly label as concept; proposed authentic team/office photograph 2400×1350, 16:9 master, safe 3:1 crop; no fabricated branding on a building |
| Gateway hero `Gemini_Generated_Image_di6xpzdi6xpzdi6x.png` and minerals hero `berbera_gateway_hero_current-1...` | P1 content verification; generic port visual is not proof of Berbera | Obtain licensed, dated identifiable Berbera photographs; same 16:9 master; caption photographer/date/permission internally; alt may name Berbera only after verification |
| Contact hero `contact_page_hero_berbera_current_v8-1...` | P2 visual softness and stray embedded text observed | Clean photographic original 2400×1350; keep quay/cranes within mobile crop; no embedded lettering; alt 'Berbera port at sunset' only if verified |
| Mineral images `mineral-gypsum-crystal-cluster.jpg`, `mineral-copper-raw-nuggets.jpg`, `mineral-gold-nuggets.jpg` | P1 relationship to actual material unverified | Real representative lot photography with scale reference and consistent neutral lighting; 1600×1200 master, 4:3; specimen photo must not be described as concentrate without proof; illustrative sample label when necessary |
| Assay/lab `Gemini_Generated_Image_h2beg6h2beg6h2be.png` | P1 provenance; P2 mismatched quarry alt | Authentic authorized sampling/lab image or visibly labeled illustration; 1600×1200, 4:3; alt describes actual visual, no invented lab affiliation |
| Source camp and assay documents `...fuxe6m...`, `...8emjbj...` | P1; generated-image filenames; documents must not imply actual certification | Licensed documentary imagery or captioned illustration; redact real sensitive identifiers; text content in HTML; report extracts only from approved records |
| Home gateway/map and `market-trade-routes-map-berbera.png` | P2; large raster map, real routes not verified | Build precise SVG diagram from licensed/geographically accurate base; text alternative in HTML; distinguish connectivity concept from active carrier service; no decorative curve implies a tested route |
| Trade workflow `Gemini_Generated_Image_ere62eere62eere6.png` | P2 raster workflow 1376×768 displayed ~1300×726 | Replace with HTML six-step process using approved copy; readable at 320px and 200% zoom; no new raster needed |
| Intelligence three cards | P2 mixed rendered 363×363 and 363×202 images | Common 16:9 editorial images, 1200×675 masters; preserve truthful crops; avoid duplication with product gallery where article needs another subject |
| Intelligence hero / homepage gateway alt | P2 same port image called professionals; map called logistics operations | Correct alt to actual subject, or use empty alt if decorative and adjacent text equivalent |
| Header/footer logos | P3 approval/retina QA | Preserve original geometry; use authorized vector where available or suitable raster densities; test DPR2 without claiming upscaling adds detail |

Suggested rendition widths: 320, 640, 960, 1440, 1920; encode AVIF/WebP with compatible fallback. Use width/height or aspect-ratio to reserve space. Lazy-load below-fold imagery, prioritize only the actual LCP candidate with `fetchpriority=high` after measuring. Budget targets (recommendations, not measured): hero ≤250KB mobile rendition, cards ≤80KB, initial page transfer ≤1MB where feasible without compromising proof/readability. Licensing/ownership is NOT VERIFIED for all media unless the company supplies a record.

## F. Accessibility and responsive verification

DOM-confirmed missing main landmarks on home and the eight non-minerals inner pages inspected through details, and minerals through dedicated inspection: all ten pages need one main content landmark. Headings skip levels in home/service cards; legal pages have duplicate h1s. Skipping a heading level is an information-architecture finding rather than automatic proof of a WCAG failure. Form label associations are a confirmed implementation gap: controls have no IDs, linked label or ARIA label in inspected trade HTML; company/country/destination/select controls appear unnamed in the tree. Screen-reader testing remains open.

Required manual tests: tab from address bar through skip link/navigation/CTA/forms/footer; visible focus throughout; Escape closes menus and returns focus; no keyboard traps; required/errors linked with aria-describedby; error summary focuses on invalid submit; alert/status for asynchronous success; labels persist after typing; native select/checkbox announced. For mineral panels either implement a real tabs pattern with arrow-key handling or accessible radio controls with correctly related panels. Visible-label click succeeded; do not report the first automated `check()` failure as a confirmed broken tab.

At the observed desktop width, measured document overflow was false for company, trade, gateway, responsible, intelligence, contact, privacy and terms; home also measured false. This does not establish mobile reflow. Test 320px for WCAG reflow in addition to requested widths, and 200%/400% zoom. No contrast score, screen-reader pass, reduced-motion pass or complete WCAG conformance is claimed.

| Width/device | Required behavior | Status |
|---|---|---|
| 375 / 390, Android Chrome and iOS Safari | Single-column cards/forms; contained image crops; 48px proposed controls; menu scroll/focus; no viewport overflow | NOT TESTED |
| 768 tablet portrait | Two-column cards only if text remains readable; route table contained and described | NOT TESTED |
| 1024 tablet landscape | Header fit or menu collapse; no compressed nav; logical reading order | NOT TESTED |
| 1363 desktop Chrome | Current public-content/DOM observations | PARTIALLY TESTED |
| 1440 desktop Chrome/Edge/Firefox/Safari | Consistent max-width, focus, forms and image fidelity | NOT TESTED |
| 1920 desktop | Content constrained to 1280px; images sufficient at DPR1/2; no excessively wide paragraphs | NOT TESTED |

WCAG 2.2 AA review reference: https://www.w3.org/TR/WCAG22/. Use target-size criterion 2.5.8 with its exceptions; 48px is the proposed design target, not the universal minimum stated by WCAG.

## G. Performance, SEO, privacy and security

**Performance:** No numerical live LCP/INP/CLS/TTFB or payload score is available. Run PSI mobile/desktop for homepage, minerals and trade, plus Lighthouse repeat runs on contact. Report median laboratory values and variability; CrUX field data may be unavailable on a low-traffic site. Target field 75th-percentile LCP ≤2.5s, INP ≤200ms, CLS ≤0.1. Do not substitute Lighthouse TBT for field INP. Record device/network/date and tool version. See https://web.dev/articles/vitals.

**SEO observations:** Unique page titles and canonical URLs were present on ten inspected pages. Canonical inner URLs end in slash; navigation links often omit it and browser ends at slash, but response-code/redirect-chain details were not measured. Homepage metadata and inspected inner-page description/OG selectors returned no description or social preview tags. No indexing guarantee follows from rendered pages; robots, X-Robots-Tag, XML sitemap and Search Console coverage are untested. Homepage robots meta only contains max-image-preview:large, not noindex. `lang=en-US` is observed, not necessarily an error for English content. Structured-data presence/eligibility needs a dedicated full check; no schema absence is asserted.

Recommended search content: buyer-led mineral sourcing through Berbera, gypsum specification qualification, copper ore versus concentrate inquiry, assay/sampling process and responsible sourcing. Opportunity pages must avoid supply certainty that evidence cannot support. Do not create thin country landing pages or fake language alternates. Add Organization markup using the truthful name, URL, authorized logo and published contact/location; no unverified legal identifiers, certifications, ratings or product offers. Use BreadcrumbList if real breadcrumbs exist; Article only for published real briefs. Product/Offer markup is deferred until actual offerings support it. Reference https://developers.google.com/search/docs/appearance/structured-data/organization.

**Public security/privacy:** HTTPS loaded; this does not certify TLS, secure hosting or absence of vulnerabilities. A cookie banner offered Customize/Reject All/Accept All; Reject All dismissed it and a reconsent control remained. Both Complianz and CookieAdmin stylesheet references were visible; this warrants checking plugin ownership/overlap, not claiming two active trackers or duplicate banners. Inspect actual requests/storage before and after each choice in an authorized QA environment. Forms' DOM method is GET, but FormLayer JS may intercept submission: inspect request transport before asserting real personal data is leaked. Require POST for both normal and asynchronous transport, safe logging and no secrets/inquiry details in URL.

Security headers, CSP, HSTS, anti-CSRF, spam controls, server sanitization, rate limiting, updates, backups, cookie blocking and delivery were NOT TESTED. Review with the developer rather than intrusive scanning. Test CSP in report-only staging first; restrict scripts/styles/images/connect destinations, introduce enforce mode once legitimate workflows pass. Review HSTS and includeSubDomains only after confirming all affected hosts support HTTPS. Add appropriate frame/referrer/content-type protections without breaking legitimate embeds. Do not infer business licensing from technical controls.

## H. Buyer conversion and lead routing

The visible contact details match the supplied reference: `info@corridorway.com`, `+252634480044`, Berbera, Somaliland. Footer email/tel/WhatsApp href strings are correct. App launching, WhatsApp account ownership/reply and mailbox delivery were not tested. No outreach occurred.

Current buyer form collects name, business email, phone, company, country, mineral, target volume, specification, destination and timeline. Add delivery basis (Incoterms rule + named location, or 'Please advise'), volume unit and frequency, material form, sampling/assay needs, and optional notes. Consider phone optional to reduce friction. Do not require confidential site coordinates or sensitive documents at first inquiry. Accept legitimate business users without arbitrary email-domain rejection. Clarify no binding offer is created.

Use visible linked Privacy Policy and Terms beside the submission notice; they are currently plain text within the inspected forms. Separate service inquiry processing from optional marketing consent; do not bundle promotional permission. Company-approved privacy/legal basis must reflect actual processing and applicable obligations.

Proposed workflow: buyer / supplier / general routes receive distinct inquiry type; create a unique reference; server validation and sanitization; accessible field errors with retained data; double-submit prevention; rate limiting and honeypot or accessible alternative; no personal inquiry data in URL/analytics; save record before sending notification; accountable trade-desk owner and backup; delivery retries and failure alert; confirmation only after accepted record; acknowledgement explicitly says qualification is pending. Marketing analytics should contain only anonymous journey events, subject to appropriate consent. Define retention with the company reviewer rather than inventing a duration.

Staging test requires a company-approved test mailbox, labeled synthetic records and suppressed real notifications. Verify browser success → stored inquiry → desk notification → test acknowledgement → reply ownership. Test unavailable mail/storage, slow connection, duplicate submit, invalid fields and no-JS fallback. No such end-to-end pass is claimed here. The live 24-hour response promise must be retained only if an owner and coverage support it.

## I. Prioritized defect register

`defect-register.csv` contains URL, section, device, exact observation, evidence, consequence, fix, owner, effort, dependencies and acceptance. All findings remain OPEN. Effort is indicative person-days, excluding content approval. P0 means immediate outage, exposure or loss confirmed; none was confirmed. P1 means high commercial/accessibility risk; P2 material usability/technical issue; P3 refinement. A missing measurement is an open verification task, not a fabricated defect.

## J. Industry benchmark — researched content patterns

| Official source retrieved 29 Sep 2026 | Observed pattern | Corridorway application | Do not imitate prematurely |
|---|---|---|---|
| https://www.trafigura.com/what-we-do/metals-and-minerals/ | Separates concentrates from refined metals; groups product applications, supply chain, responsible-sourcing objectives, real dated news and documented case study links | Separate product forms; explain exact service and evidence gate; publish dated approved briefs/policies | Owned transport concessions, scale metrics, financing or case studies without Corridorway evidence |
| https://www.glencore.com/what-we-do/marketing | Explains sourcing, physical movement and customer value; navigation separates products, responsible sourcing, suppliers and contacts | Clarify trading office role, partner responsibilities and buyer/supplier journeys | Global owned-asset network, investor pages, producer claims and transaction financing assumptions |
| https://www.ixmetals.com/ | Clear business/responsibility/contact groups; product portfolio, reports/policies, dated news and actual external LinkedIn destination | Make contact easy; replace placeholder social links; publish concise real documents and a credible portfolio | Global footprint, turnover, bank relationships and quantitative scale claims without verified records |

These are editorial and navigation comparisons from official retrieved text, not claims of visually measured superiority or cross-browser benchmark testing. Three strong relevant reference firms were used; a smaller industrial-material supplier benchmark remains a useful next research extension.

## K. Transformation roadmap

| Window | Actions / accountable discipline | Exit criterion |
|---|---|---|
| Immediate triage | Trade lead reviews active/verified badges, unsupported exact gypsum/route/mandate statements and pseudo-documentary imagery; developer checks inquiry delivery in staging | No inconsistent readiness claim remains; P1 risks either corrected and retested or explicitly held from publication |
| Days 1–7 stabilization | Front end fixes label associations, landmarks, product-sheet destination, 11 fragments, social placeholders, linked notices, duplicate legal titles; editor removes empty Read more; developer verifies transport/routing | Buyer/supplier/general journeys pass approved staging tests; desktop and 375/390 screenshots; P1 closure evidence attached |
| Days 8–30 improvement | Brand owner approves token system; consolidate mineral content; authenticate media; normalize cards; SEO metadata and sitemap review; accessibility/manual device tests; performance baseline and fixes | No P1 open; P2 navigation/content defects closed; measured AA criteria and CWV status documented, including field-data availability |
| Days 31–60 | Structured evidence record workflow, reviewed product sheets, real dated brief, lead assignment and failure monitoring; optimize images/fonts/plugins based on measurements | Every commercial claim has source/owner/date; clear records and lead follow-up ownership |
| Days 61–90 refinement | Add country/language content only if demand and staffing support it; improve inquiry completion using approved analytics; recurring evidence/route reviews; independent accessibility assessment | Decisions based on actual conversion/quality data; no simulated metrics; full regression matrix and responsible sign-off |

Quick wins: true labels/links, heading and alt corrections, claim qualification, removal of placeholders. Architecture: shared data-driven status model, semantic forms, evidence workflow and authenticated document access. Retain working CMS/theme elements where fixes suffice.

## L. Developer-ready handoff

No repository access was available. Do not assume a file path exists merely because an asset URL names a theme or plugin. The browser references `corridorway-flagship` theme CSS and FormLayer, CookieAdmin and Complianz assets; the maintainer must map them to source templates and plugin settings in their authorized checkout. Never edit WordPress core/vendor files to solve template issues.

Implement tokens in the maintained theme design system; one header/footer template; reusable mineral/status cards; forms with unique per-form IDs and server-backed POST; proper main landmarks; standard article cards. Use the section D table as page-level requirements. Add anchor targets only for real sections; canonical slash URLs in new internal links; set scroll-margin-top if sticky navigation is later adopted. Header remains clean with logo, seven links and primary trade CTA, without a new contact strip. Mobile menu needs a named toggle, aria-expanded, reliable close behavior and focus management. Footer retains contact details and only working supported sections/social profiles.

### Proposed metadata copy (approval required)

| Page | Title | Description |
|---|---|---|
| Home | Corridorway Minerals Trade Office — Berbera Mineral Sourcing | Discuss mineral sourcing, specification requirements and qualification with Corridorway Minerals Trade Office in Berbera, Somaliland. |
| Company | Company & Approach — Corridorway Minerals Trade Office | Learn about Corridorway's role, qualification approach and approved company information. |
| Minerals | Mineral Opportunities & Qualification — Corridorway | Explore mineral sourcing opportunities and the evidence required before specifications, availability and commercial terms are confirmed. |
| Trade | Submit a Mineral Buyer or Supply Inquiry — Corridorway | Share mineral specifications, quantity, destination and timeline, or present a supply opportunity for qualification. |
| Gateway | Berbera Gateway & Mineral Logistics — Corridorway | Understand the proposed logistics process through Berbera and request route-specific transport information. |
| Responsible | Responsible Mineral Trade & Verification — Corridorway | Understand the source, authority, sampling and documentation checks used to qualify mineral opportunities. |
| Intelligence | Mineral Trade Intelligence — Corridorway | Read sourced mineral and logistics briefs when published. |
| Contact | Contact Corridorway — Berbera, Somaliland | Contact Corridorway by email, phone, WhatsApp or inquiry form to discuss a buying requirement or supply opportunity. |
| Privacy / Terms | Privacy Policy / Terms of Use — Corridorway | Read Corridorway's approved privacy notice / website terms. |

SEO descriptions are drafts, not descriptions currently observed. Add approved Open Graph/Twitter preview metadata with licensed imagery and truthful page descriptions.

### Evidence register specification and publication gates

Required internal fields: claim ID, exact text, URL/section, claim class, source record, lot/site/material, dry/wet basis, issue date, expiry/review date, reviewer, approval state, NDA/public-disclosure scope and superseded version. Public summary: status, basis, last reviewed, access method; private documents need not be exposed wholesale.

Separate **verified supply** (source-specific approved authority, assay/specification, quantity/readiness), **sourcing opportunity** (under qualification), and **regional potential** (published occurrence reference, no supply promise). Record verification per check; a pending authority/assay cannot silently inherit a homepage Active status. Do not change gypsum to 98% because it was mentioned earlier: the live ≥90% statement and any replacement require actual current lot assays. This audit does not independently certify either grade.

Proposed safe homepage lead: 'Corridorway Minerals Trade Office supports mineral sourcing inquiries, source qualification and Berbera-connected trade coordination.' Use only after company confirms those capabilities. Evidence-stack heading: 'What we check before an offer.' Copper: 'Copper sourcing opportunity. Material form, grade and availability are subject to source and assay qualification.' Gold: 'Gold and precious mineral inquiries are subject to source, authority, assay and compliance review.' Catalog editorial instructions should become straightforward status descriptions rather than commands such as 'Include as ... only unless ...'.

## M. QA and release acceptance

1. Create staging backup of database, media, theme, plugin settings and relevant configuration; verify restore procedure and preserve current production URLs. Staging must not send real leads; protect sensitive data and prevent staging indexing.
2. For each issue, record before evidence, staging build/version, owner, exact change and retest result. No automatic CLOSED state from a code commit alone.
3. Retest all 10 discovered pages and any additional sitemap URLs; all links and fragments resolve to intended content; no placeholder profiles, downloads or article destinations.
4. Inspect 375/390/768/1024/1440/1920 and 320px reflow; iOS Safari, Android Chrome, desktop Chrome/Edge/Firefox/Safari; test menus, anchors, images, tables, forms, zoom and orientation. Record actual device/browser versions.
5. Run axe or equivalent and manual keyboard/screen-reader checks; validate names, landmarks, headings, focus, contrast, target size, errors and motion. An automated zero is not full conformance.
6. Execute approved synthetic buyer/supplier/general form scenarios, request transport inspection, storage/notification/acknowledgement, failure/retry, invalid input and anti-spam checks. Confirm no inquiry content enters URLs or anonymous analytics.
7. Verify image subject/provenance, rights, alt and responsive rendition quality; no generated art presented as actual company operations or certificates.
8. Run lab performance baselines/retests and separately report available field CWV; validate canonical/title/meta/social/schema, robots/sitemap/404 and redirect behavior with actual HTTP tooling.
9. Company trade lead signs material claims; brand owner approves tokens and master assets; qualified reviewer approves applicable privacy/legal disclosures; developer signs technical checks.
10. User authorization is required before production publication. Deploy a tagged approved build during agreed window; verify buyer/contact paths and critical pages immediately. Roll back if lead routing fails, critical navigation breaks, content is wrong or a material accessibility regression appears.
11. Post-release: same-day desktop/mobile smoke test; within 48 hours compare screenshots, metadata and performance; at 7 days inspect actual lead handling and logs; at 30 days review available field data, indexing and claim freshness. Recheck time-sensitive routes and lot availability on their approved cadence.

### Scorecard methodology and status

Each category is scored 0–10 only when its full criteria have adequate coverage. Criteria below have equal weight within a category; overall category weights sum to 100. Tests missing essential coverage mean UNTESTED for scoring even when specific defects were observed. Rubric: 0–2 severe systemic failure, 3–4 major gaps, 5–6 usable with material defects, 7–8 verified good with minor gaps, 9–10 all applicable checks documented and no material unresolved defects.

| Category | Overall weight | Equal-weight measurable criteria | Current score |
|---|---:|---|---|
| Brand Consistency | 8 | Approved master comparison; token match; repeated components; responsive consistency | UNTESTED — approved master and responsive QA missing |
| Visual Design | 8 | Reading order; image purpose; hierarchy; desktop/mobile balance | UNTESTED — responsive visual review missing |
| Typography | 6 | Computed family/size; readable density; zoom/reflow; consistent heading scale | UNTESTED — zoom/reflow missing |
| Layout Cohesion | 6 | Shared grids; sibling alignment; spacing; six-width stability | UNTESTED — six-width stability missing |
| Images & Media | 8 | Subject/alt accuracy; provenance; crop/retina; delivery | UNTESTED — provenance/payload/mobile missing |
| Navigation | 8 | Destination accuracy; menu keyboard/touch; route coverage; no dead ends | UNTESTED — sitemap and touch/keyboard missing |
| Mobile UX | 10 | 375/390 layouts; controls; form flow; device matrix | UNTESTED |
| Accessibility | 10 | Automated criteria; keyboard/focus; screen reader; contrast/reflow | UNTESTED — confirmed gaps but full test coverage missing |
| Performance | 10 | Lab LCP/CLS; field INP where available; asset analysis; repeat tests | UNTESTED |
| SEO | 6 | Crawl/index; metadata; internal semantics; schema/social/404 | UNTESTED — technical crawl incomplete |
| Content Credibility | 8 | Cross-page status consistency; identifiable proof; accurate product forms; claim owner/date | UNTESTED — private proof records unavailable; public contradictions confirmed |
| Buyer Conversion | 8 | Entry clarity; qualified fields; accessible validation; actual delivery/routing | UNTESTED — end-to-end delivery missing |
| Public Security/Privacy | 4 | HTTPS/header behavior; consent blocking; secure forms; actual processing notice | UNTESTED — transport/headers/consent blocking missing |

**Overall numeric score withheld.** No fully tested category meets its coverage gate; public desktop findings are sufficient to prioritize work but insufficient for a defensible weighted international-standard score. Untested categories are not treated as zero or ten.

### Evidence map and source limits

`evidence/home.json`: homepage DOM measurements, text, links and metadata. `evidence/pages.json`: nine inner-page content snapshots, IDs, canonical tags and form structures. Its main-scoped heading/image arrays are empty because these pages lack a main landmark; this is not absence of images/content. `evidence/details.json`: subsequent whole-document inspection for eight inner pages, excluding minerals, including image/field/landmark/overflow observations. Minerals has dedicated browser DOM/AX evidence quoted in this report and captured screenshot; its image records appear in the manifest based on that inspection. Ten `.jpg` files provide desktop screenshots. Screenshots are point-in-time evidence, not responsive tests; natural dimensions and rendered sizes correspond to the observed state and can change after deployment.

Research references retrieved: WCAG 2.2 (W3C), Web Vitals (Google web.dev), Organization structured data (Google Search Central), and three official benchmark pages in section J. No proprietary content/assets were copied. Berbera depth/route claims were flagged for company/operator verification; no replacement numerical value was independently established. No reserves, customer names, licences, partnerships or transaction history were invented.
