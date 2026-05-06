## Project Structure
| File | Purpose |
|------|---------|
| `catalogue_file_generation.py` | Step 1 — Generates the dummy 108-row product catalogue dataset |
| `catalogue_final_audit.py` | Step 2 — Runs the quality audit and completeness scoring |
| `catalogue_audit_report.xlsx` | Step 3 — Final formatted Excel output with 3-tab report |
# Catalogue Quality Audit Tool

A Python-based audit tool built for e-commerce/B2B catalogue operations.
Automatically evaluates product listing quality across key attributes and
generates a formatted Excel report for catalogue managers.

## What It Does
- Detects duplicate SKU IDs across the catalogue
- Flags missing values across 9 critical listing fields
- Identifies short or incomplete product descriptions
- Calculates a completeness score (%) for every SKU
- Exports a 3-tab Excel report with color-coded quality flags

## Output Report Structure
| Tab | Contents |
|-----|----------|
| Summary Dashboard | Overall metrics + missing values per field |
| Full Audit Detail | All SKUs with scores and color-coded flags |
| Action Required | Isolated Poor and Duplicate listings only |

## Tech Stack
- Python (pandas, openpyxl)
- Excel (output format)

## Business Context
Built to simulate real catalogue auditing workflows in B2B software
listing environments — where maintaining data completeness, avoiding
duplicate entries, and ensuring listing quality at scale are core
operational responsibilities.

## Sample Output
| Metric | Value |
|--------|-------|
| Total SKUs Audited | 108 |
| Duplicates Found | 8 |
| Good Quality | 11 |
| Needs Review | 47 |
| Poor Quality | 42 |
| Avg Completeness Score | 83.4% |
