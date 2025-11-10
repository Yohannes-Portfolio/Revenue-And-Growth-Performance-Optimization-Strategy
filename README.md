# Revenue Growth Performance & Optimization Strategy

## Table of Contents

- [Project Background](#project-background)
- [Data Structure & Initial Checks](#data-structure--initial-checks)
- [Executive Overview](#executive-overview)
- [Deep Dive Insights](#deep-dive-insights)
  - [Growth Driven by Customer Volume, Not Transaction Value](#growth-driven-by-customer-volume-not-transaction-value)
  - [Revenue Is Highly Concentrated in Morning Hours](#revenue-is-highly-concentrated-in-morning-hours)
  - [Cyclical Revenue Pattern: End-of-Month Decline](#cyclical-revenue-pattern-end-of-month-decline)
  - [Extreme Product Concentration and Transaction Value Variation](#extreme-product-concentration-and-transaction-value-variation)
- [Recommendations](#recommendations)
  - [Optimise Operational Hours and Staffing](#optimize-operational-hours-and-staffing)
  - [Streamline Product Portfolio](#streamline-product-portfolio)
  - [Address End-of-Month Revenue Decline](#address-end-of-month-revenue-decline)
  - [Increase Average Transaction Value](#increase-average-transaction-value)
- [Caveats & Assumptions](#caveats--assumptions)

---

## Project Background

This specialty coffee startup, launched in 2022, has rapidly built a loyal customer base through its retail location offering coffee, tea, bakery items, and specialty drinks.

The business achieved breakthrough growth in the first half of 2023, with revenue surging 94% and transaction volume increasing 103% over the six-month period. As the startup scales, understanding revenue patterns and operational efficiency has become critical. This project analyzes six months of granular transaction data to identify actionable insights that can sustain rapid growth while optimizing operations for profitability.

Insights and recommendations focus on three key areas:

- **Temporal Revenue Patterns:** Hourly, daily, and monthly sales analysis to optimize staffing allocation and inventory management

- **Product Portfolio Performance:** Product-level revenue analysis to identify top drivers and opportunities to streamline operations

- **Operational Optimization:** Data-driven recommendations to sustain growth while improving margins through cost reduction and resource allocation

A link to the interactive dashboard made in Tableau for this sales anallysis can be found [here.](https://public.tableau.com/views/CoffeeSales_17624595519230/CoffeeShopSalesDashboard?:language=en-GB&publish=yes&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link).

The Excel Workbook used to clean and analyse this data including a cleaning Log can be downloaded [here.](https://github.com/Yohannes-Portfolio/Revenue-And-Growth-Performance-Optimization-Strategy/blob/main/Coffe%20Sales%20Project%20Workbook.zip)

## Data Structure & Initial Checks

The coffee shops transaction database as seen below consists of a single table with detailed point-of-sale records, containing a total of **149,116** transaction records across six months (January-June 2023).

<p align="center">
  <img width="427" height="574" alt="image" src="https://github.com/user-attachments/assets/652239c8-80f2-4cc6-959a-941a470aa762" />
</p>

Before analysis was begun data cleaning operations involved the elimination of duplicate transactions and date/range time validation to ensure consistency in the data.
<p align="center">
  <img width="1866" height="179" alt="image" src="https://github.com/user-attachments/assets/cd8ea566-a45a-4200-9641-ed454c178e71" />
</p>

## Executive Overview

Analysis of the first half of 2023 transaction data reveals three critical patterns limiting profitability despite volume growth of **103% in total revenue**. **Morning hours from 8am to 11am generate 45% of daily revenue**, while evening hours contribute less than 10%, creating a severe efficiency mismatch. **Just 15 products types drive 90% of revenue**, while 30 product types are maintained, distributing operational complexity across items that deliver minimal return. **A predictable monthly 28.6% revenue decline from the 26th to 29th** is linked to customer paycheck cycles. These three patterns remained constant over the six-month timeframe and are, therefore, structural customer behaviors, not one-off anomalies.

Below is the overview for sales for the tableau dashboard, more visuals are given and explained throughout the report. The interactive dashboard can be found [here.](https://public.tableau.com/views/CoffeeSales_17624595519230/CoffeeShopSalesDashboard?:language=en-GB&publish=yes&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link)

<p align="center">
  <img width="1514" height="804" alt="image" src="https://github.com/user-attachments/assets/afaae270-e5fb-4e7e-8499-35f84e292293" />
</p>

## Deep Dive Insights

### Growth Driven by Customer Volume, Not Transaction Value

**Revenue growth of 94% was driven almost entirely by transaction volume growth of 103%, while average transaction value remained flat at $4.90** throughout the six-month period. Revenue increased from $370K in January to $719K in June exclusively through serving more customers rather than increasing spending per customer.

### Revenue Is Highly Concentrated in Morning Hours

- **The window in the morning, between 8 am and 11 am, generates 45% of the total daily revenue.** It includes a peak hour at 10 am, which contributes 12.7% of total revenue. This concentration is stable over the course of the week as seen by the darkest cells clumping in the same morning hours whether it is Monday or Saturday.

- **Time of day drives the revenue performance, whereas the day of week has little effect on it.** There is a horizontal consistency in the heatmap, as each row just shows similar patterns. Customer behavior follows daily routines rather than weekday versus weekend distinctions.

- **Afternoon hours, 11 am to 5 pm, account for 40% of the day's revenue but function at a much lower productivity level**, with an average of 6% revenue per hour, contrasted to 11.46% per hour in the morning hours between 8-11. Morning hours are almost twice as productive as afternoon hours on an hourly basis.

- **Evening hours from 6 p.m. to 8 p.m. are dead time with minimal activity, together accounting for less than 10% of daily revenues.** The hour of 8 p.m. contributes a mere 0.42% of overall daily revenue, with hourly values as low as £0.34K, while being the lightest cells on the heatmap across all days. Such a critical drop shows that the business is operating in a period of very low demand from customers, keeping operation capacity while bringing negligible return.

<p align="center">
  <img width="793" height="652" alt="image" src="https://github.com/user-attachments/assets/55fdc9c7-7e7f-4b02-9a50-8c32d8084c39" />
</p>

## Cyclical Revenue Pattern: End-of-Month Decline

- **Revenue exhibits a consistent cyclical pattern with a 28.6% average decline in the final days of each month, peaking mid-month before declining sharply from the 26th through the 29th**. The drop is reached on the 28th in February and the 29th in all other months, with an immediate recovery on the first day of the next month. This pattern repeats across all six months with remarkable consistency.

- **This end-of-month decline reflects customer monthly financial cycles tied to paycheck schedules and budget constraints**. Customers in early-to-mid month, when budgets are fresh, spend more liberally on discretionary items such as specialty coffee, then as month's end approaches, before the next paycheck, reduce non-essential purchases. The immediate recovery every month start confirms this is cyclical cash flow behavior rather than declining customer interest or operational problems.

- **Over the period of six months, this cyclical pattern remained in place, suggesting that it is real and deeply ingrained into customer financial behavior**, rather than business operations. This creates predictable low-revenue periods from the 26th to 29th of each month.

<p align="center">
  <img width="1235" height="680" alt="image" src="https://github.com/user-attachments/assets/d5823db2-4803-450f-8279-a0b21026b867" />
</p>

### Extreme Product Concentration and Transaction Value Variation

- **Revenue is strongly concentrated among only a few products: Barista Espresso represents 13.3% of total revenue, Brewed Chai Tea accounts for 11.1%, and Hot Chocolate brings in 10.7%**. These top three products contribute more than 35% of the total revenue and the top 13 products account for 90% of all revenue.

- **The bottom 14 product types make up only 10% of total revenue** while the business runs close to 30 different product types, with those beyond the top 15 each accounting for less than 2% apiece.

- **This revenue concentration pattern remained stable over the six-month growth period, despite 106% transaction volume increase**. The relative positions of the top products did not change, nor did their revenue share, which suggests that new customers have similar product preferences to existing customers. The same 12 to 15 products accounted for 90% of revenue in each of the six months.

<p align="center">
   <img width="1242" height="628" alt="image" src="https://github.com/user-attachments/assets/7d38c67d-cb7c-4f79-ab1c-38c5340982a1" />
</p>

## Recommendations

### Optimize Operational Hours and Staffing

- **Reduce or eliminate evening operations between 6pm and 8pm to save costs during the worst-performing period**. Evening hours account for less than 10% of daily revenues, and the 8pm hour is responsible for as little as 0.42% of total revenue at values as low as £0.34K total revenue. The **operations team** should consider shutting down at 6pm or running with a skeleton crew during evening hours to cut labor and overhead costs while sacrificing very little revenue.

- **Provide dynamic staffing schedules that mirror hourly revenue patterns**. The store managers should concentrate staffing during the morning peak window from 8am to 11am when 45% of daily revenue is generated, reduce staffing during afternoon hours since productivity drops to half that of morning hours, and minimize evening staffing. This reallocation helps with matching labor costs to revenue generation, which also provides assurance of service quality at peak moments.

### Streamline Product Portfolio

- **Remove the last 10 to 15 products generating only 10% of revenue**. Products after the top 15 each generate less than 2% of revenue individually and unnecessarily complicate the operations disproportionately. The **product management team** should remove low performers to uncomplicate operations, decrease ingredient waste, and free up the staff to upsell core products driving 90% of revenue.

- **The focus of marketing efforts and staff training should be on the 12 to 15 core products** that continuously generate 90% of the revenue. The **marketing team** should develop campaigns around the top three products-Barista Espresso, Brewed Chai Tea, and Hot Chocolate-which drive 35% of revenue. Staff training should include staff development programs for upselling proven winners rather than promoting underperforming items.

### Address End-of-Month Revenue Decline

- **Launch focused promotions during the predictable low-revenue period of the 26th through 29th of every month**. The **marketing team** should introduce value-oriented promotions such as discounted combo deals or loyalty bonuses to counteract the consistent 28.6% revenue decline during these days when customer budgets tighten before paychecks. Simultaneously, the supply chain team should reduce perishable inventory orders in this period to minimize waste and improve margins.

### Increase Average Transaction Value

- **Implement strategic upselling to increase per-customer spending**. Average transaction value remained flat at approximately $4.90 throughout the six-month period despite 106% volume growth. Store managers should train staff to suggest premium versions, size upgrades, or add-ons for core products, particularly during the high-traffic morning window. The **finance team** should analyze profitability by product within the core 15 revenue drivers to identify pricing optimization opportunities.

## Caveats & Assumptions

The analysis and recommendations are based on the following assumptions and limitations:

- Six-month timeframe: Data covers January-June 2023 only. Seasonal patterns outside this period (summer, holidays) are not captured and may differ from observed trends.

- Revenue focus only: Cost data (COGS, labor, overhead) was not available. Financial modeling incorporating margin analysis is recommended before implementation.

- Stable external conditions: Analysis assumes relatively consistent external factors (weather, competition, local events). Significant environmental changes may alter customer behavior patterns.

- Implementation capacity: Recommendations assume operational capability to execute changes (staffing, space, technology).
