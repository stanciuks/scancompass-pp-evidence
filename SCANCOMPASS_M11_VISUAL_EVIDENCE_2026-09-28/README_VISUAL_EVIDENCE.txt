SCANCOMPASS — M11 VISUAL ACCEPTANCE / DEFECT EVIDENCE
Date: 2026-09-28

Screenshots 14 and 15 record a live defect found after M11 closure:
- the newly-created shared report opens successfully;
- clicking "Download this report" then reaches /api/reports/download but returns
  "This report cannot be downloaded".

This strongly indicates that the download submission is not carrying the share capability
correctly, or that the download request path is otherwise rejecting it.

No share capability/token value is included in these screenshots.

The M11 closure tag remains historical and must not be moved. The defect should be fixed
through a separate post-M11 hotfix before M12 implementation proceeds.
