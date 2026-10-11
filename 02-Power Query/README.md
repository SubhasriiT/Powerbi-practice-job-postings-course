# Part 2: Power Query

[← Back to main README](../README.md)

Covers the Power Query chapter of Luke Barousse's Power BI course: getting data in, cleaning it, and shaping it into a model. I rebuilt each lesson myself, one `.pbix` file per section. Dataset: `job_postings_flat` (about 479,000 data job postings), split into fact and dimension tables in the Project #2 files.

## Files
- 📁 `Images/`: screenshots of every page
- 📊 Five Power BI reports (open with Power BI Desktop):

| File | Pages | What it covers |
|------|-------|----------------|
| `Power Query Intro Section.pbix` | Web - Nominal GDP, Folder Data Jobs | Loading a table from a web page; combining a folder of monthly files so new files load on refresh |
| `Power Query Editor Section.pbix` | Date Inspection, Salary Inspection | Fixing date-time vs date columns; converting hourly pay to yearly (× 2080) to compare salaries |
| `Project 2 & Merge.pbix` | Company Stats, Skills Stats, Schedule Type Stats, Group By | Star schema (fact + dimension tables), relationships and cross-filter direction, splitting columns into rows, conditional columns, merge, Group By |
| `Append Section.pbix` | Append - Excel Sheets | Appending 12 monthly Excel sheets into one table (479K postings) |
| `M Language Section.pbix` | Salary Stats | Column from Example, custom columns, salary buckets |

## Page Gallery

| | |
|---|---|
| ![Web - Nominal GDP](Images/Web%20-%20Nominal%20GDP.png)<br>**Web - Nominal GDP**<br>Table pulled straight from a web page, shown as a map and a ranked bar chart | ![Folder Data Jobs](Images/Folder%20Data%20Jobs.png)<br>**Folder Data Jobs**<br>Monthly files combined from a folder: job count by title and monthly trend |
| ![Date Inspection](Images/Date%20Inspection.png)<br>**Date Inspection**<br>Same column before and after converting date-time to date only | ![Salary Inspection](Images/Salary%20Inspection.png)<br>**Salary Inspection**<br>Median yearly vs hourly salary adjusted to a yearly figure (hourly × 2080) |
| ![Company Stats](Images/Company%20Stats.png)<br>**Company Stats**<br>Top companies by job count and by median salary, using the company dimension table | ![Skills Stats](Images/Skills%20Stats.png)<br>**Skills Stats**<br>Top skills and their median salaries, using the skills tables and a both-direction cross-filter |
| ![Schedule Type Stats](Images/Schedule%20Type%20Stats.png)<br>**Schedule Type Stats**<br>Job counts and median salary by schedule type, from a new schedule dimension table | ![Group By](Images/Group%20By.png)<br>**Group By**<br>Skill counts per job title from a Group By query instead of a huge merged table |
| ![Append - Excel Sheets](Images/Append%20-%20Excel%20Sheets.png)<br>**Append - Excel Sheets**<br>Twelve monthly sheets appended into one table: 479K jobs over time | ![Salary Stats](Images/Salary%20Stats.png)<br>**Salary Stats**<br>Combined yearly + adjusted hourly salary, and hourly salary buckets built with Column from Example |

## What I learned
- **ETL basics:** Power Query extracts, transforms, and loads, and every step is saved and re-runs on refresh.
- **Import vs DirectQuery:** import is fast but makes big files; DirectQuery keeps files small but is slow.
- **Star schema:** one fact table plus dimension tables; many-to-one relationships; why a filter can fail until cross-filter direction is set to both.
- **Reference vs duplicate:** reference reuses earlier steps instead of repeating them.
- **Cleaning:** replace values, trim, split column by delimiter into rows, conditional columns, unpivot.
- **Append vs merge:** append stacks tables; merge joins them. I walked through all six join types.
- **Group By:** aggregating with counts keeps files much smaller than a merged flat table (about 76 MB down to 39 MB in the course demo). Medians of medians are misleading, so stick to counts.
- **M language:** every click in the editor writes M code. Column from Example and custom columns can build new fields, and an AI chatbot can help debug errors.

## What I followed vs changed
- Followed the course builds for all five sections.
- Applied a purple theme to the visuals.

## Next
➡️ Part 3: DAX (coming soon)
