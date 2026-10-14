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
