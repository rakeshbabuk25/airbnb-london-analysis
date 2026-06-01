# London Airbnb Market Analysis

## Overview
This project analyses whether London represents a viable short-term 
rental market for a real estate management company considering 
expansion. The analysis covers pricing, occupancy rates, and 
revenue performance across London boroughs using publicly available 
data from Inside Airbnb.

## Business Task
Identify which London neighbourhoods offer the strongest revenue 
potential for short-term rentals, and determine what factors 
(room type, superhost status, location) drive performance.

## Data Source
- **Source:** Inside Airbnb (insideairbnb.com/get-the-data)
- **Dataset:** London listings CSV
- **Rows after cleaning:** [your number here]
- **Key columns used:** neighbourhood_cleansed, room_type, price, 
  estimated_revenue_l365d, estimated_occupancy_l365d, 
  host_is_superhost, review_scores_rating
- **License:** Creative Commons CC0

## Tools Used
| Tool | Purpose |
|---|---|
| Google Sheets | Data cleaning and preparation |
| Tableau Public | Visualisation and dashboard |

## Data Cleaning Steps
1. Removed columns not relevant to the business task (kept 20 of 75)
2. Stripped `$` and `,` from the price column and converted to numeric
3. Deleted rows with blank values in: id, host_id, price, room_type, 
   neighbourhood_cleansed, estimated_revenue_l365d
4. Flagged and removed price outliers below £10 and above £1,000 per night
5. Retained rows with blank review scores (new listings with no reviews)

## Key Findings
- Lambeth generates the highest average annual revenue at £21,777, 
  outperforming Westminster (£16,809) and Kensington & Chelsea (£15,367)
- Superhosts earn 2.5x more than non-superhosts (£19,242 vs £7,630 
  avg annual revenue)
- Entire homes/apartments average 61 occupied days per year vs 33 for 
  hotel rooms, making them the most consistently booked room type
- City of London is the only borough where private rooms (£360.69/night) 
  price higher than entire homes (£354.32/night)
## Dashboard
View the live Tableau dashboard here: [paste your Tableau Public link]

![Dashboard Preview]
<img width="1417" height="834" alt="Screenshot 2026-05-31 at 21 32 07" src="https://github.com/user-attachments/assets/0c6d8591-2e7d-4faf-8232-ee095233f769" />


## Next Steps for Further Exploration
- Combine with seasonal calendar data to identify peak booking months
- Add competitor pricing data from other platforms
- Analyse the impact of minimum night requirements on occupancy

## Author
Rakesh Babu Kancharla
