DEPARTMENTAL EXTERNAL LINKAGE PLAN — SECTION 2 DASHBOARD
This is a separate dashboard from the prior UOL Progress Report.
Dataset: 107 cleaned activity-plan entries from 15 original submissions.
9 overlapping DELP51/DELP52 entries and 2 null placeholders were excluded during source cleaning.
Start the dashboard by running START_DASHBOARD.bat (Python installed), or run `python -m http.server 8000` in this directory and open http://localhost:8000.
Opening index.html by file:// may prevent browser fetch of data.json.
Charts use a CDN copy of Chart.js. The dashboard still provides textual chart fallbacks if the CDN cannot load.
Filters: Semester, Faculty, Department, Activity Type, Partner, Submission, free-text search. Exports filtered data as CSV; Download PDF generates a paginated PDF report offline using the included pdf-export.js. No PDF CDN libraries are required.
Source Excel included as Section2_Cleaned_Source.xlsx. No new activity entries were added.

Submission count now reads submission-roster.json (15 original forms), separately from data.json (107 cleaned activities). DELP51 duplicate-only and DELP18/DELP19 placeholder-only remain in the submission roster but not activity totals.

Semester coverage note: Two roster-only submissions (DELP18, DELP19) lack a recorded source semester and contain no retained activity. They are included in Fall 2026 institutional coverage totals to keep 7 faculties and 13 departments visible; their original source semester fields remain blank. Charts and activity percentages are based on the 107 recorded Fall 2026 plans only.


LIVE EXCEL CONNECTION (UPDATED): The dashboard reads Section2_Cleaned_Source.xlsx directly each time it starts and when Reload Excel is clicked. The workbook now contains two source-of-truth tabs: Cleaned Section 2 (one row per retained plan) and Dashboard Submission Roster (one row per original submission, including forms without retained plans). Edit/save the XLSX IN THIS DASHBOARD FOLDER, then click Reload Excel or reload the page. If hosting on GitHub Pages, upload/commit the edited XLSX and reload the deployed page after deployment; browser pages cannot automatically write back to an Excel file. The included data.json and submission-roster.json are legacy snapshot backups, not live inputs. Keep submission refs unique in the roster, and add new submissions to the roster before adding their activity rows. Source audit counts 118/9/2 refer to the original historical cleanup and are not recomputed from new entries.

CROSS-DEVICE DATA LOADING (2026-10-16): The published JSON snapshot is loaded FIRST on every device, including iPhone Chrome/Safari. The Excel workbook is optional via Reload Excel. When editing the XLSX, regenerate BOTH data.json and submission-roster.json before publishing, then upload the entire folder to GitHub Pages. Use the updated index.html and app.js together (cache-busting release token).
