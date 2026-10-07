SCANCOMPASS — CURRENT-MAIN REDESIGN SCREENSHOT EVIDENCE
Date: 7 October 2026

Four screenshots covering what is NEW in the current-main integration of
direction D: the two download controls side by side after the real-PDF work
merged, the M12C domain page in the design's own language, and the Domains
link that appears only for a signed-in visitor. They are a selection from the
fifteen integration captures committed on the branch. The full set and the
written record stay in the source repository; see
SCANCOMPASS_VISUAL_REDESIGN_CURRENT_MAIN_PP_Evidence_2026-10-07.txt.

NOT MERGED, NOT DEPLOYED. Draft PR #28 against main. These show a draft branch
served locally in production mode with network responses scripted in the
browser — not the live site. The ten screenshots in
SCANCOMPASS_VISUAL_REDESIGN_2026-10-05/ cover the earlier exploration and the
original implementation on draft PR #18, which is also still unmerged.

  01-report-with-pdf-and-html-controls-dark.png
      The shared assessment report with BOTH download controls in the header
      action row — "Download PDF" first, then "Download HTML report" — after
      M12D's real PDF endpoint was merged into the redesign. Both buttons read
      the same in-memory capability at click time; neither the page markup nor
      any request URL carries it. The host name is fictional and the report
      data is real pipeline output from the application's own assessment code.
      The score sits in a sentence with the measuring rule beside it, and
      coverage is presented separately and explained as completeness rather
      than confidence — the distinction the old interface blurred.

  02-m12c-domains-page-gate-closed-light.png
      The M12C domain page in direction D, in the light theme, with the feature
      gate CLOSED. Every domain route answers 404 and the page shows its own
      unavailable notice. This is the state that proves the redesign changed
      presentation only: the page still decides for itself, and the closed gate
      still wins.

  03-account-signed-in-domains-link-focus-dark.png
      The account page, signed in, with the new Domains panel under the sign-in
      panel and keyboard focus on the "Manage domains" link, showing the focus
      ring. The link is rendered only after the session request reports a
      signed-in visitor, so it never appears in server-rendered markup.

  04-account-signed-out-no-domains-link-light.png
      The same page signed out: the sign-in form, and NO link to the domain
      page. This is the counter-case for screenshot 03, and the reason the link
      was put in the account panel rather than the site header. It is also the
      page that screenshot 02 of the 2026-10-05 set showed as effectively
      invisible before the redesign — the fields, labels and hints are now
      there.

DELIBERATE EXCLUSION
The branch also carries captures of the domain page showing an ISSUED
VERIFICATION CHALLENGE, including the DNS record name and its value. Those
values are scripted test data, not real ones, but they are shown in the
position where a REAL one-time verification value would appear. Following the
project's rule that one-time verification values are never reproduced in
Personal Project evidence, NONE of those captures is included here, and the
gate-closed view was selected instead. The real production verification value
the owner published was never supplied to any assistant session and does not
exist anywhere in this repository.

SANITIZATION
No account exists in these captures and none of these pages was signed in to
with a real credential; the sign-in form is empty. No email address, token,
capability value, password, database URL, connection string, host identifier or
provider key appears in any image. No real third-party website is shown. No
backend, worker or database was involved: the session, domain and
report-resolution endpoints were intercepted in the browser.

AI ASSISTANCE
The integration, the restyled domain page, the navigation link and these
captures were produced by Claude, an AI coding assistant. The direction, the
request for a navigation link and the storage exception were the owner's
decisions. The owner's own visual review of PR #28 is recorded, with its
provenance, in section 9 of the evidence note beside this file.

END OF EVIDENCE
