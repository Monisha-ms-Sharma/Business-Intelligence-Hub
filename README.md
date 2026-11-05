# Business-Intelligence-Hub
Turn raw data into business intelligence — right in your browser.
https://ai-bi-hub.lovable.app

Business Intelligence Hub is a self-service analytics web app for business owners and analysts. Upload one or many data files and instantly get exploratory data analysis, an automatically detected data model, interactive KPI dashboards, nine types of business analysis, AI-written findings, forecasts and machine-learning segments, a formatted PDF report, and a place to embed your published Power BI and Tableau reports.

# Who it is for
Business owners and managers who need quick answers from spreadsheets without writing code
Business analysts who want a fast first look (EDA) before formal modeling
BI developers preparing and cleaning data for Power BI or Tableau
Students and educators learning analytics concepts with real data
Small teams without a dedicated data platform

# Why it was made
Getting from a raw file to a useful insight usually means juggling Excel, Python or R scripts, and a BI tool. This app brings those first steps into one place: upload, understand, model, analyse, ask, forecast, and present. No installation, no account, and no need to write code.

# What it can do
1. Multi-format, multi-file upload
CSV, TSV, TXT, JSON
Excel (.xlsx, .xls, .xlsm) — every sheet becomes its own table
Parquet
ZIP folders containing any of the formats above
Several files at once (for example a fact table plus its dimension tables)
A built-in 3-table sample retail model to try instantly
2. Exploratory Data Analysis (EDA)
Histograms: distribution and skew of any numeric field
Box plots: spread, median and outliers, optionally split by a category
Scatter plots: relationships between two fields with a fitted trend line and R²
3. Semantic data model, relationships and automatic joins
Automatic detection of key columns shared across tables (name matching plus value overlap)
Cardinality detection: one-to-one, many-to-one, many-to-many
Tables classified as Fact, Dimension or Standalone
An interactive diagram: drag tables, click relationships for details
Automatic joins: related tables are flattened into one wide "Joined model" table, so dashboards and analyses can use dimension attributes (region, category, format) alongside fact measures without writing any join code
4. Interactive KPI dashboards
KPI cards (total, average, change vs. prior period) for each measure
Trend over time, share by category, and breakdown charts
Measure, breakdown and filter selectors that update every chart
5. Core types of business analysis
Type	What it answers	How
Descriptive	What happened?	Total, mean, median, mode, std dev, segment comparison, trend
Diagnostic	Why did it happen?	Driver correlations, under-performing segments, anomalies (>3σ)
Predictive	What is likely next?	Linear time-series trend with a 3-period forecast
Prescriptive	What should we do?	Recommended actions plus a what-if simulation slider
Inferential	Is it significant?	95% confidence intervals, Welch t-test between segments
Causal	What causes it?	High vs. low driver effect comparison (observational)
Mechanistic	How does the system work?	Multiple regression with standardized effects and R²
Quantitative & Qualitative	Numbers and composition together	Numeric summary combined with category mix
Text / content	What are people saying?	Word themes and positive/neutral/negative sentiment
6. AI analyst
Narrative insights: a written briefing of the most important findings, recommended actions and caveats
Ask a question: type anything about the data ("Why did returns rise in Q3?") or pick a suggested question
Answers are grounded in a computed statistical summary plus a few sample rows — the full dataset is never sent
Results are marked as AI-generated so you can check key numbers against the Dashboard and Analysis tabs
7. Forecasting and machine learning
Holt-Winters forecast with trend and 12-month seasonality (falls back to a linear trend when history is short)
ARIMA(p,1,0) forecast with typical error and a 3/6/12-month horizon
Decision-tree model showing which fields drive a measure, with accuracy (R²) on unseen rows
k-means clustering that groups similar records into segments you can size and describe
8. Data quality checks
Missing values, duplicate rows, mixed date/number formats, extra spaces and inconsistent capitalisation
A 0–100 quality score with High / Medium / Low severity per issue
Download the full results as CSV, or download the table with duplicate rows removed
9. Compare two datasets
Pick a baseline and a comparison (for example last month vs. this month)
Rows, shared / added / removed columns and changed column types
Totals, means, medians and missing counts side by side, with % change highlighted
New and disappeared category values
10. PDF report
One click opens a formatted report ready to save as PDF
Includes summary cards, automatic findings, the AI narrative if generated, dashboard charts, quality results and column profiles
11. More tools
Column profile: type detection, missing values, unique counts, statistics
Correlation grid across all numeric fields
Chart studio: bar, line, area, pie and scatter charts
Data preview with clean CSV export (ready for Power BI or Tableau)
12. Power BI and Tableau public embeds
Paste a Power BI Publish to web link or iframe code
Paste a Tableau Public view link
View the published report next to your analysis

# How to use it
Open the app and drop one or more files (or click Try a sample retail model).
Choose a table from the selector at the top. The largest table is chosen first; the Joined model table is added automatically when tables relate to each other.
Explore the tabs: Dashboard → Analysis → AI analyst → Forecast & ML → EDA → Data model → Quality → Compare → Profile → Charts → Data → Power BI & Tableau.
Click PDF report to save or share the findings, or export clean data from Data and build your report in Power BI or Tableau.
Privacy
Files are read in your browser and are never uploaded to a server for storage.
Refreshing the page clears the session; nothing is saved between visits.
The only data that leaves your device is the AI analyst request: a computed statistical summary and up to 15 sample rows are sent through the app's AI service to generate the briefing or answer. Column names, aggregate figures and those sample rows appear in that request, so avoid pasting sensitive data you would not want summarised.
No account, no tracking of your files, no uploads kept on a server.

# Limitations
Very large files (hundreds of MB or millions of rows) may be slow or run out of browser memory.
One table at a time: dashboards and analyses run on the selected table. The automatic Joined model covers the common fact-plus-dimensions case; arbitrary multi-fact or many-to-many joins are not flattened.
Relationship detection is heuristic. It relies on similar column names and shared values, so unusual naming may be missed or mismatched.
Statistics are simplified: p-values use a normal approximation, the Analysis tab's forecast is linear, and causal results are observational (not proof of cause).
Forecasts need a date column with at least 4 months of data; seasonality needs 24+ months. ARIMA needs a longer history than Holt-Winters.
Machine learning is basic: the decision tree uses up to 8 numeric features and complete rows only; k-means needs numeric fields and is sensitive to outliers.
Text sentiment uses a small English word list, not a full language model.
AI answers can be wrong. They are generated from a summary, not the full data, and should be checked against the Dashboard and Analysis tabs. AI use depends on workspace credits.
Embeds are public views only. Private Power BI or Tableau reports that need sign-in are not supported.
No saved sessions, user accounts or sharing. Work is lost on refresh.
Excel formulas are read as their stored values. Charts and pivot tables inside workbooks are ignored.
Python and R are not run; the equivalent statistics are computed in the browser.
PDF export uses the browser's print dialog, so page breaks and chart placement can vary by browser.

# Possible future enhancements
Live connections to Power BI semantic models per signed-in user
Saved projects, user accounts and shareable dashboard links
Scheduled AI findings briefings (weekly digests)
SQL-style query builder across several tables
Live connections to databases and cloud warehouses
Export of the joined model and quality results back into Power BI / Tableau dataflows

