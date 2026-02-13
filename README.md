# Ride Cancellation Analysis 

## Problem Statement

A ride-hailing platform experiences order failures when customers don't successfully get a car. This project analyzes failed orders to identify key failure patterns—including cancellations
(before/after driver assignment) and rejections—and investigates how these failures vary by time of day. By examining metrics like cancellation timing and estimated time of arrival (ETA),
this project aims to uncover operational insights that could improve match success rates and customer experience.

## Tech Stack
 Language: Python
 Libraires: Numpy, Pandas, Matplotlib
 Visualization: Excel

## Data Description
<img width="876" height="445" alt="Screenshot 2026-02-13 140127" src="https://github.com/user-attachments/assets/2c0fa479-e512-4cd2-8900-2427633cb089" />

### Key Insights
- <img width="325" height="101" alt="image" src="https://github.com/user-attachments/assets/1ddd36e6-cf49-4075-aa01-88280b12d456" />
- <img width="452" height="352" alt="image" src="https://github.com/user-attachments/assets/ad292473-71d7-4873-9616-946c2eb683bf" />


- A large portion of failures (42%) happen **before any driver is assigned**, showing that customers lose patience when they don’t quickly see a match.
- **8 AM is the most critical hour**, where all failure types spike equally, indicating the system is overwhelmed by demand.
- **Late-night hours (9 PM–3 AM)** suffer mainly due to **driver shortages**, not lack of riders.
- Customers are willing to wait **twice as long** once a driver is assigned, proving that *visibility and reassurance* play a major role in user behavior.
- System rejections remain consistently high across all hours, suggesting **rigid matching rules** may be limiting successful rides.

## Root Cause Hypothesis & Business Recommendations

| Problem Area | Root Cause | Business Impact | Recommended Action |
|-------------|------------|-----------------|--------------------|
| Morning Rush (8 AM) | Demand exceeds available drivers | High lost revenue during peak hours | Introduce peak-hour incentives and surge pricing to increase driver supply |
| Late Night (9 PM–3 AM) | Low driver availability | Large number of abandoned rides | Night shift bonuses and minimum earnings guarantees |
| Pre-Assignment Cancellations | Slow matching or low supply | Customers leave before seeing any driver | Improve matching speed and show real-time ETA early |
| System Rejections | Overly strict matching rules | Artificial ride failures | Relax constraints during high demand |
| Post-Assignment Cancellations | Poor driver ETA or ride quality | Customer dissatisfaction | Better driver positioning and quality scoring |

## ETA hour Analysis

<img width="452" height="352" alt="image" src="https://github.com/user-attachments/assets/272166b2-0e87-422d-b343-967470ebbeb8" />

- From this plot we can see that the average ETA is highest during the morning rush (7–9 AM), peaking around 8 AM, showing that demand exceeds driver availability. A smaller peak appears in the evening (5–7 PM) due to office return traffic. Late-night and early-morning hours have lower ETAs, indicating better supply-demand balance. Overall, ETAs closely follow real-world commuting patterns.

## Business Outcome

Most ride failures are **not technical problems** — they are **operational problems**.  
The platform loses the most value when customers don’t quickly see a driver. Improving **driver availability, faster matching, and better communication** can significantly increase completed rides without increasing demand.


## 🧱 Tech Stack

| Layer        | Technology            |
|--------------|------------------------|
| Language     | Python                 |
| Libraries    |  Pandas, Numpy, Matplotlib |
| Visualization | Excel                |




