## Problem
A 105-row employee dataset needed to be usable for analysis — but categories, names, dates, 
and contact info were inconsistent enough that formulas and pivot tables would silently produce wrong results.

## Understanding the data
- Department and City had up to 3 spelling/casing variants per category (Sales/sales/SALES)
- Salary was stored three different ways — plain numbers, text with commas, text with a currency prefix
- Joining Date used four different formats, some genuinely ambiguous (03/05/2025 = 3rd May or 5th March?)
- 5 Salary values and 21 Email values were missing
- 4 rows were exact duplicates

## Approach
- TRIM() + PROPER() to fix casing and stray spaces in names
- Find & Replace (Match Case) to standardize Department and City spellings
- SUBSTITUTE() + VALUE() to convert Salary into consistent numbers
- DATEVALUE() to auto-parse unambiguous dates, manual review for ambiguous ones
- Missing Salary/Email values flagged as "Not Found" rather than left blank or guessed
- Remove Duplicates to eliminate exact duplicate rows

## Solution
105 raw rows → 100 clean records
13 Department spelling variants → 5 standardized categories
5 missing salaries and 21 missing emails flagged, not hidden
4 duplicate rows removed

Files: raw_data_100.xlsx (original) and 01_data_cleaning_project.xlsx (cleaned, with scorecard and charts)
