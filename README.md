Business Intelligence Hub
Turn raw data into business intelligence — right in your browser.

App: https://aibihub.app/(opens in a new tab)
Publisher: AI BI Hub

<img width="1920" height="973" alt="Business Intelligence Hub" src="https://github.com/user-attachments/assets/b3f689b5-9b8f-492e-85ef-f942ada2bc5f" />


Business Intelligence Hub is a self-service analytics web app for business owners, analysts, and data professionals. Upload one or many files to explore every row, build automatic or custom data models, create KPI dashboards, investigate business performance, run statistical analysis, forecast outcomes, and export reports. Public Power BI and Tableau reports can also be displayed alongside the analysis.

Who it is for
Business owners and managers who need clear, actionable answers from spreadsheets without writing code
Business analysts who want a fast exploratory analysis before formal modeling
Data analysts and BI developers preparing, profiling, cleaning, and documenting data
Students and educators learning analytics with realistic sample datasets
Small teams that need browser-based analysis without building a data platform
Why it was made
Getting from a raw file to a useful answer usually means moving between spreadsheets, statistics code, and a BI tool. Business Intelligence Hub brings those first steps together: upload, understand, connect, analyze, forecast, customize, and present.

Every analysis page offers both:

Plain-English View — everyday language, business meaning, and practical next steps
Technical View — data-science terminology, methods, statistical detail, and analyst next steps
Switching views keeps the user on the same page with the same selections. Calculations use the full filtered dataset, never a sampled subset. Tables and charts may limit how many rows or categories they display, but those display limits do not reduce the records used in calculations.

What it can do
1. Multi-format, multi-file upload
Supported inputs:

CSV, TSV, and TXT
JSON, including Data Profiler session files
Excel (.xlsx, .xls, .xlsm) — each populated sheet becomes a table
Parquet
Feather v2 and Arrow IPC (.feather, .arrow, .ipc)
SQL dumps containing INSERT INTO … VALUES rows
XML with repeated record elements and flattened nested fields
Text-based PDF tables
Word .docx tables — each table becomes a dataset
ZIP archives containing supported files
Multiple files at once, such as a fact table and its dimension tables
Legacy .doc and Feather v1 files must be re-saved in a supported format. Scanned or image-only PDFs are not supported.

2. Built-in sample dataset models
Try a Sample Dataset Model opens fictional datasets with 1,200 main-table records each. Most include linked lookup tables; Geospatial and Entertainment are single-table samples.

Available categories:

Finance & Banking
Healthcare & Medical
E-commerce & Retail
Cybersecurity & Vulnerability
Corporate Performance & Strategy
Human Resources & Payroll
Business Analysis · Project Delivery
Business Analysis · Operations & KPIs
System Analysis · Performance & Reliability
System Analysis · Requirements & Testing
Space & Aviation
Engineering & Manufacturing
Biotech & Biosciences
Geospatial & Location
Food & Tourism
Media & Entertainment
Samples open every non-AI feature for free, do not require sign-in, and do not consume a free analysis. Healthcare-like data also triggers a privacy reminder before analysis.

3. Data Profiler interoperability
Import from Data Profiler provides step-by-step instructions and accepts:

data-profiler-session.json to import every saved table
Data Profiler's For BI Hub model (CSV, all rows) export for individual tables
All imported records stay on the device. To move results back, download the BI Hub Excel workbook and use Import from BI Hub in Data Profiler.

4. Automatic and custom data models
Detect shared keys using column-name similarity and value overlap
Inspect matched, unmatched, blank, and repeated keys across all rows
Identify one-to-one, one-to-many, many-to-one, and many-to-many relationships
Classify tables as fact, dimension, or standalone
Drag tables around an interactive relationship diagram
Generate joined models while retaining unmatched main-table rows
Choose star, snowflake, fact-constellation, or custom layouts
Select multiple main tables for shared-group models; each becomes a separate analysis so totals are not mixed
Add, edit, validate, download, reset, and apply custom relationships
Automatic models remain available for free. Custom modeling is included with samples and eligible free full analyses, then requires paid access for new datasets.

5. KPI dashboards and interactive visuals
KPI cards with totals, averages, and period comparisons
Trends, category shares, and grouped breakdowns
Page-wide date and category filters applied consistently across the workspace
Chart tooltips, clickable bar filters, and linked selections
Up to three levels of drill-down on supported native visuals, with Back and reset controls
Clear notices when a visualization cannot be produced from the available data
6. Tracking Measures and user-defined formulas
Infer a likely subject domain from column-name tokens
Explore the measure catalog by domain
Search measures and filter for candidate or missing column matches
Show the formula, matched columns, calculated result, and records used when suitable data exists
Create custom measures with aliases, one or more columns, built-in calculations, custom expressions, and optional percentage formatting
Edit or remove saved measures and override a listed measure's formula by using the same name
User-defined measures are calculated from all rows and saved privately in the signed-in user's workspace. They are not shared with other users or added to a public App Library.

7. Business Insights
Dedicated views cover:

Targets: KPI goals, directional targets, and RAG status
What changed: period-over-period variance by business group
80/20: Pareto concentration and the groups contributing most of a result
Customers: RFM segmentation and monthly cohort retention
Drop-off: conversion funnels from yes/no steps or an ordered stage column
Best / worst case: scenario forecasts, ranges, and what-if adjustments
Findings cite actual groups and values. Statistical evidence includes the p-value and record count where applicable; associations are not presented as proof of cause.

8. Statistical Analysis, Time Series, and Text & Sentiment
The Analysis area includes:

Analysis	What it provides
Descriptive	Totals, mean, median, mode, standard deviation, distributions, groups, and growth
Diagnostic	Numeric associations, segment gaps, and unusual records
Time Series	Trend, seasonality, residuals, anomalies, autocorrelation, and period growth
Predictive	A three-period trend forecast or a regression-based estimate
Prescriptive	Data-linked next steps and a what-if sensitivity slider
Inferential	Confidence intervals and Welch two-sample Student t-tests
Causal	Observational high/low comparisons with explicit non-causal caveats
Mechanistic	Multiple linear regression, standardized coefficients, and R²
Quantitative & Qualitative	Numeric outcomes compared across categorical groups
Text & Sentiment	Themes, sentiment classes, trends, group comparisons, and example comments
Sentiment scoring uses an in-browser DistilBERT-SST-2 transformer through a Web Worker. The model is downloaded once and inference stays on the device. Provisional or fallback word-list scoring is clearly identified if the model is loading or unavailable.

9. Forecasting and machine learning
Holt-Winters forecasting, with 12-month seasonality when sufficient history exists
ARIMA(p,1,0) forecasting with a 3-, 6-, or 12-month horizon
Decision-tree regression with feature importance and held-out R²
k-means clustering on selected standardized numeric fields
Missing-month detection that pauses forecasting rather than silently compressing time or inventing values
10. Exploratory Data Analysis and column profiling
Histograms, box plots, scatter plots, fitted lines, and R²
Column types, null counts, distinct counts, summary statistics, and outliers
Correlation grid across eligible numeric columns
Dense scatter plots bin all points rather than dropping records
Data dictionaries with inferred roles, meanings, examples, and warnings
11. Data quality and preparation
Missing values, exact duplicates, mixed date/number formats, whitespace, and case inconsistencies
A 0–100 quality score with High, Medium, and Low severity issues
Optional trimming, deduplication, case standardization, ISO dates, empty-row removal, and null handling
Cleaning creates a separate dataset and leaves the original untouched
Download quality results, deduplicated data, and the data dictionary
12. Dataset comparison
Compare a baseline and comparison dataset
Review row counts, shared, added, and removed columns, and changed types
Compare totals, means, medians, missing counts, and percentage changes
Identify new and disappeared category values
13. Saved views, downloads, and reports
Save and reopen reviewed views with their displayed charts, choices, and explanations
Download reviewed analysis as HTML
Export an Excel workbook with summary, column statistics, dictionary, quality results, grouped analysis, and all data rows
Create an executive one-pager and print or save it as PDF
Open the full PDF report through the browser's print dialog
Export clean CSV data for use elsewhere
Standard downloads identify Publisher: AI BI Hub.

14. Customize Results
The white-label report builder supports:

Organization name, report title, preparer, footer, brand color, and logo
Data-source names, links, reporting periods, and notes
Plain-English or technical report content with selectable sections
PDF and HTML downloads
Device sharing, email-draft creation, and links to common cloud drives
Customized downloads deliberately omit the app and publisher name. Email drafts cannot attach files automatically; users download the result and attach it themselves.

15. Power BI and Tableau public embeds
Paste a Power BI Publish to web URL or iframe snippet
Paste a Tableau Public view link
View and interact with the published report inside BI Hub
These controls do not edit Power BI or Tableau reports, formulas, models, or queries. Editing remains in the source product. Public embeds are not a substitute for secure private-report sharing.

Free access
Sample datasets include every non-AI feature without sign-in or consuming a free analysis.
Your first 3 full dataset analyses are free per signed-in user.
Free analyses are limited to one account per user or device.
After the included analyses, DIY tools lock for new datasets. Standard analysis, filters, saved views, and downloads remain free.
AI is paid-member-only at all times.
Guests can purchase without signing in, then claim access with a verified account using the same email address as checkout.

How to use it
Open aibihub.app(opens in a new tab) and drop one or more files, choose Import from Data Profiler, or select Try a Sample Dataset Model.
Choose the active table from the table selector. Related files also produce an automatic joined model.
Set page-wide date or category filters. Every downstream page uses all matching rows.
Explore Dashboard, Business Insights, Analysis, What Comes Next, Explore, How Files Connect, Data Health, Prepare Data, Compare, Column Facts, Make a Chart, Your Rows, and Power BI & Tableau. Technical View shows the corresponding technical names.
Switch between Plain-English View and Technical View without losing the current page or selections.
Save reviewed views, download Excel/CSV/HTML results, open the PDF report, or use Customize Results for white-label output.
Use Back to Home to keep a resumable analysis. Use Reset to restore analysis settings without deleting loaded tables. In the workspace, the logo offers a confirmed hard reset that clears the analysis session and returns Home; the landing-page logo is static.
Privacy and session behavior
Files are parsed and analyzed in the browser. Uploaded records are not sent to the backend for storage.
Automatic calculations, joins, statistics, forecasts, machine learning, sentiment inference, and report generation run on the device.
AI requests send a compact statistical profile computed from all rows, not individual data rows. That profile can include column names, category values, aggregate figures, and trends, so sensitive datasets should be reviewed before using AI.
Sign-in, paid access, payment verification, AI allowances, free-analysis enforcement, and saved custom-measure definitions use backend services. Payment details are handled by the checkout provider.
Free-analysis enforcement stores account usage and a hashed IP address to apply the account/device limit.
Saved custom measures are private to their owner and persist in that user's workspace. Uploaded data, filters, calculated columns, saved views, custom report drafts, and custom model designs are session state and are cleared by refresh or a confirmed hard reset.
Data Profiler session files contain records and should be handled privately, even though the transfer itself stays on the device.
See the app's Privacy Notice, Terms & Conditions, and Refund Policy for the governing terms.
