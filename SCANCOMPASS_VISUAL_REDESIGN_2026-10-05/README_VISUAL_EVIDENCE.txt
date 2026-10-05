SCANCOMPASS — VISUAL REDESIGN SCREENSHOT EVIDENCE
Date: 5 October 2026

Ten representative screenshots covering the whole redesign, from the interface
that was rejected to the implemented direction. They are a selection from the
42 images curated on the implementation branch, which were themselves reduced
from 189 captures. The full set and the written record stay in the source
repository; see SCANCOMPASS_VISUAL_REDESIGN_PP_Evidence_2026-10-05.txt.

NOT MERGED, NOT DEPLOYED. Draft PR #18 against main. These show a draft branch,
not the live site.

  01-before-main-landing-desktop.png
      The landing page as it was on main. The framework's starter typeface, one
      weight ramp for every heading, tracked uppercase micro-labels, and the
      score and coverage presented as two equal headline numbers.

  02-before-main-account-desktop.png
      The sign-in page as it was on main, and the clearest single defect: under
      the CSS framework's preflight the Email and Password inputs have no
      border or background, so the form is effectively invisible. Compare
      screenshot 09.

  03-exploration-b-course-light-landing.png
      Direction B, "Course", at revision 1 — light, before the owner asked for
      a dark site.

  04-exploration-b-course-dark-landing.png
      The same screen at revision 2, after the owner's instruction that the
      site should be dark. This is the lineage the owner went on to choose.

  05-prototype-d-landing-desktop.png
      Direction D, "Course + Evidence": the static prototype built from B's
      frame and C's evidence language, after the owner said they liked B and C.
      SCANCOMPASS is in capitals at the owner's instruction. THE OWNER
      EXPLICITLY SELECTED D.

  06-implementation-landing-desktop-dark.png
      D implemented in the real application, dark (the default). Production
      build, strict content-security policy.

  07-implementation-landing-desktop-light.png
      The same page with the light theme, which the owner asked for as an
      option alongside the dark default.

  08-implementation-report-desktop-dark.png
      The full assessment report. The course is the server's own fix order, not
      a re-sorting; yellow marks only values the assessment recorded; blue
      marks only confirmed protections; every colour is beside a word. The host
      name is fictional and the report data is real pipeline output generated
      by the application's own assessment code.

  09-implementation-account-desktop.png
      The sign-in page after the redesign — the same page as screenshot 02,
      with visible fields, labels and hints.

  10-implementation-persisted-light-reload.png
      The theme-persistence proof: a remembered light theme after a FULL
      RELOAD, with no frame in which it paints dark. The mechanism is a nonce'd
      script whose body is a module constant, under one narrowly scoped and
      test-pinned storage exception approved by the owner. Zero policy
      violations were observed in any case tested, including one in which every
      framework script was blocked.

Sanitization: no account exists and none of these pages was signed in to. The
forms are empty. No email address, token, capability value, password, database
URL, host identifier or provider key appears in any image. No real third-party
website is shown.

AI assistance: the audit, the directions, the implementation and these captures
were produced by Claude, an AI coding assistant, using the frontend-design
skill. The direction and the storage exception were the owner's decisions.

END OF EVIDENCE
