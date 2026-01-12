# MercadoLibre Funnel and Retention Analysis

## Project Overview
This project analyzes user behavior for MercadoLibre, focusing on the **conversion funnel** and **retention cohorts**. The goal is to identify drop-off points, calculate conversion rates, and evaluate user retention over time.

## Description
The analysis was performed using SQL and Excel in three stages:

1. **Explore Tables**: Examined the structure of `mercadolibre_funnel` and `mercadolibre_retention` tables and explored event types to understand user actions.  
2. **Deconstruct Funnel**: Built multi-step conversion funnels using SQL CTEs, counted users per stage, calculated conversion rates, and segmented metrics by country.  
3. **Retention and Cohort Analysis**: Measured accumulated active users and retention percentages (D7, D14, D21, D28) by country, defined monthly user cohorts, and calculated cohort retention.  

All SQL queries, instructions, and results are documented via **screenshots**, as the original dataset is not available. An Excel file summarizes key findings in an **executive-friendly dashboard**.

## Tools
- SQL (TripleTen simulator)
- Excel (for executive dashboard)

## Project Structure

### 01_explore_tables
| # | Task | Screenshot |
|---|------|------------|
| 1 | List columns and data types of `mercadolibre_funnel` | 01_funnel_table_schema.png |
| 2 | List columns and data types of `mercadolibre_retention` | 02_retention_table_schema.png |
| 3 | Explore unique event types in the funnel | 03_event_types_preview.png |

### 02_deconstruct_funnel
| # | Task | Screenshot |
|---|------|------------|
| 4 | Create CTEs for each funnel stage and count users | 04_funnel_cte_part1.png, 04_funnel_cte_part2.png, 04_funnel_cte_result.png |
| 5 | Calculate conversion rates between stages | 05_conversion_rates_part1.png, 05_conversion_rates_part2.png, 05_conversion_rates_part3.png, 05_conversion_rates_result.png |
| 6 | Segment funnel conversions by country | 06_conversion_by_country_part1.png, 06_conversion_by_country_part2.png, 06_conversion_by_country_part3.png, 06_conversion_by_country_result.png |

### 03_retention_cohorts
| # | Task | Screenshot |
|---|------|------------|
| 7 | Count accumulated active users by country (D7, D14, D21, D28) | 07_accumulated_active_users.png |
| 8 | Convert counts to retention % by country | 08_retention_pct_by_country.png |
| 9 | Define user cohorts by signup month (YYYY-MM) | 09_user_cohorts.png |
| 10 | Calculate cohort retention for D7, D14, D21, D28 | 10_cohort_retention_part1.png, 10_cohort_retention_result.png |
