# Power BI Practice — Data Job Postings Dashboard (Guided Course Project)

## About this project
This is a **learning/practice project** built while following [Luke Barousse's "Power BI for Data Analytics - Full Course for Beginners"](https://www.youtube.com/watch?v=FwjaHCVNBWA) on YouTube. I'm using it to build hands-on Power BI skills — DAX-free visual design, interactivity, and dashboard layout — alongside my primary BI tool, Tableau.

This is **not an original independent analysis**. The dataset, business questions, and most chart designs come directly from the course. I've noted below exactly what I followed as-is versus what I changed or added myself.

## Dataset
`job_postings_flat` — a global data-job-postings dataset (used throughout the course) containing fields such as `job_title`, `job_country`, `salary_year_avg`, `salary_hour_avg`, `job_skills`, `job_work_from_home`, `job_no_degree_mention`, and `job_posted_date`.

## Preview

### Project #1: Data Jobs Dashboard
![Data Jobs Dashboard](Images/Project%201%20-%20Data%20Jobs%20Dashboard.jpg)

### Project #1: Job Title Drill Through
![Job Title Drill Through](Images/Project%201%20-%20Job%20Title%20Drill%20Through.jpg)

## Page Gallery

| | |
|---|---|
| ![Column and Bar Charts](Images/Column%20&%20Bar%20Charts.jpg)<br>**1. Column & Bar Charts**<br>Bar, clustered column, stacked and 100% stacked charts comparing median salaries and no-degree postings by job title | ![Line and Area Charts](Images/Line%20&%20Area%20Chart.jpg)<br>**2. Line & Area Charts**<br>Job posting trends across 2024, with trend lines, drill-down, stacked area, and a column + line combo chart |
| ![Common Charts](Images/Common%20Charts.jpg)<br>**3. Common Charts**<br>Pie, donut, treemap and scatter plot showing no-degree share, WFH share, job types, and hourly vs yearly salary | ![Map Charts](Images/Map%20Charts.png)<br>**4. Map Charts**<br>Bubble map and filled map showing where data jobs are posted globally |
| ![Uncommon Charts](Images/Uncommon%20Charts.jpg)<br>**5. Uncommon Charts**<br>Ribbon chart for salary rank over time, plus waterfall and funnel charts | ![Tables and Matrices](Images/Tables.jpg)<br>**6. Tables & Matrices**<br>Table with star-rating measure and icons, plus matrices with data bars, gradients and sparklines |
| ![Cards](Images/Cards.jpg)<br>**7. Cards**<br>Card, new card, multi-row card, gauge and KPI visuals for headline salary numbers | ![Slicers](Images/Slicers.jpg)<br>**8. Slicers**<br>List, dropdown and date and salary range slicers with a clear-all-slicers button | |

## Files
- 📁 `Images/`: screenshots of every page
- 📊 `Visualization Section.pbix`: the full Power BI report (open with Power BI Desktop)

## Progress: Part 1 complete — Visualizations chapter + Project #1

| Page | Chart types | What I did |
|------|-------------|------------|
| 1. Highest Paying & No-Degree Jobs | Bar chart, clustered column, stacked bar, 100% stacked bar | Followed the course build exactly |
| 2. Job Trends in 2024 | Line chart, area chart, stacked area chart | Followed the line/area chart builds from the course; **added the stacked area chart ("What is trend of data job in 2024?") myself** — the technique was taught in the course but this specific visual wasn't built by the instructor, so I applied it independently |
| 3. Common Chart Types | Pie chart, donut chart, scatter plot, treemap | Followed the course build, but **changed the color theme/palette** from the original |
| 4. Global Job Postings (Maps) | Dot map, filled/shape map | Course covers 3 map types including an ArcGIS map; **I completed 2 of 3** — the ArcGIS map returned an error on my setup, which appears to require Power BI Premium (the instructor mentions this as a possible limitation) |
| 5. Uncommon Charts | Ribbon chart, waterfall chart, funnel chart | Followed the course build; changed the color theme/palette |
| 6. Tables & Matrices | Table, matrix, star-rating quick measure, conditional formatting (data bars, icons, gradients), sparklines | Followed the course build; changed the color theme/palette |
| 7. Cards | Card, new card, multi-row card, gauge, KPI | Followed the course build |
| 8. Slicers | Vertical list, tile, dropdown, between-range slicers, sync slicers, clear-all-slicers button | Followed the course build |
| 9. Buttons & Bookmarks | Page navigator, back/home button, bookmark-controlled slicer toggle | Followed the course build |
| **Project #1: Data Jobs Dashboard** | KPI cards, trend line, scatter plot, bar chart, matrix table + a **drill-through page** per job title | Followed the course structure and layout principles; applied a custom purple theme throughout |

## What I'm learning next
Continuing through the course from here:
- Power Query (data import, advanced transformations, Append vs Merge, M language)
- DAX (Explicit Measures, Parameters)
- Course Project #2 (Dashboard Build, Share Dashboard)
- After the course: building a Power BI project from a self-chosen dataset and business question, independent of the course

## Why this is here
I'm building my Power BI skills alongside my primary tool (Tableau). This repo is a transparent record of that learning process — not a portfolio centerpiece. My independent, original analysis projects are pinned separately on my profile.

## Tools
Power BI Desktop

