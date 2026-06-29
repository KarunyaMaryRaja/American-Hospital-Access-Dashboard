# American-Hospital-Access-Dashboard
An Excel-based data analysis project identifying hospital desert counties across the United States using real government data from CMS and the U.S. Census Bureau.

# Project Overview
This project analyzes **5,432 Medicare-certified hospitals** across the U.S. to answer one critical public health question:
"Which American counties have large populations but critically limited access to hospitals — and how good is the care in those hospitals?"
Two government datasets were combined, cleaned, and analyzed to produce an interactive Excel dashboard that reveals hospital access disparities, quality gaps, and ownership patterns across all 50 states.

# 🔍 Key Findings

| Metric | Value |
|--------|-------|
| Total hospitals analyzed | 5,432 |
| National avg star rating | 3.2 / 5.0 |
| Hospitals with emergency services | 83% |
| Hospital desert counties identified | 373 |

# Top 10 States by Hospital Count
| Rank | State | Hospitals |
|------|-------|-----------|
| 1 | Texas (TX) | 468 |
| 2 | California (CA) | 378 |
| 3 | Florida (FL) | 221 |
| 4 | Ohio (OH) | 196 |
| 5 | Illinois (IL) | 194 |
| 6 | New York (NY) | 191 |
| 7 | Pennsylvania (PA) | 187 |
| 8 | Louisiana (LA) | 161 |
| 9 | Indiana (IN) | 151 |
| 10 | Georgia (GA) | 149 |

# Top 10 States by Avg Star Rating
| Rank | State | Avg Rating |
|------|-------|------------|
| 1 | Utah (UT) | 4.24 ★ |
| 2 | Colorado (CO) | 3.96 ★ |
| 3 | South Dakota (SD) | 3.89 ★ |
| 4 | Wisconsin (WI) | 3.78 ★ |
| 5 | Minnesota (MN) | 3.77 ★ |
| 6 | Virginia (VA) | 3.68 ★ |
| 7 | Ohio (OH) | 3.58 ★ |
| 8 | Idaho (ID) | 3.55 ★ |
| 9 | Rhode Island (RI) | 3.55 ★ |
| 10 | Nebraska (NE) | 3.50 ★ |

### Top 10 States with Most Hospital Deserts
| Rank | State | Desert Counties | Severity |
|------|-------|----------------|----------|
| 1 | North Carolina (NC) | 31 | 🔴 Critical |
| 2 | Texas (TX) | 24 | 🔴 Critical |
| 3 | Louisiana (LA) | 23 | 🔴 Critical |
| 4 | Tennessee (TN) | 20 | 🟠 High |
| 5 | Virginia (VA) | 19 | 🟠 High |
| 6 | Ohio (OH) | 17 | 🟠 High |
| 7 | Alabama (AL) | 15 | 🟠 High |
| 8 | Michigan (MI) | 15 | 🟠 High |
| 9 | New York (NY) | 15 | 🟠 High |
| 10 | Pennsylvania (PA) | 10 | 🟡 Moderate |

# Workbook Structure

| Sheet | Purpose |
|-------|---------|
| `Raw_Hospitals` | Original CMS data — 5,432 hospitals, untouched |
| `Raw_Population` | U.S. Census 2025 county population data |
| `State_Ref` | 50-state lookup table (full name ↔ abbreviation) |
| `Merged_Data` | Both datasets joined via nested XLOOKUP |
| `Analysis` | All advanced formulas — COUNTIFS, AVERAGEIFS, RANK |
| `Pivot_Tables` | Ownership breakdown and desert county pivot tables |
| `Dashboard` | Final interactive dashboard with KPI cards and charts |

## Excel Skills Used

| Skill | Where Applied |
|-------|--------------|
| `XLOOKUP` (nested) | Join population to hospital data via State + County |
| `COUNTIFS` | Count hospitals and desert counties per state |
| `AVERAGEIFS` + `IFERROR` | Average star rating excluding nulls and errors |
| `RANK` | Rank all 50 states by hospital count |
| `IF` + `AND` + `COUNTIFS` | Flag hospital desert counties |
| `Power Query` | Data import, cleaning, null handling, type conversion |
| `PivotTables` | Ownership and desert county summaries |
| `State Reference Table` | Lookup table to resolve state format mismatch |
| `Sheet Protection` | Lock dashboard from accidental edits |

# Data Sources
Hospital General Information | CMS | [data.cms.gov](https://data.cms.gov/provider-data/dataset/xubh-q36u) |
County Population Estimates 2025 | U.S. Census Bureau | [census.gov](https://www.census.gov/data/tables/time-series/demo/popest/2020s-counties-total.html) |

# Key Insight
North Carolina, Texas, and Louisiana have the highest number of hospital desert counties — yet Texas also has the most hospitals overall. This reveals that **raw hospital count does not equal equitable access.**

**Karunya Mary Raja**
MS in Information Systems & Technologies — University of North Texas
