# Singapore HDB Resale Trend Analysis Using Python

## Project Overview
This repository contains an exploratory data analysis (EDA) and visualization project focused on the Singapore Housing & Development Board (HDB) resale property marketThe analysis bridges raw historical property records with data visualization techniques to uncover trends, price growth trajectories, and structural relationships within the housing market.

Historically viewed as uniform public housing utilities, the Singapore public housing market has evolved to behave like a mature, competitive asset class with distinct foundational and luxury-tier segments.

---

## Project Objectives
* **Track Town Trajectories:** Monitor and track town-by-town price growth trajectories across Singapore.
* **Property Valuation Dynamics:** Analyze how property valuations scale over the years.
* **Quantify Resale Price Index:** Analyze the resale price index to quantify market movements.
* **Assess Structural Influences:** Evaluate how flat types, architectural models, and physical size influence final resale prices.
* **Lease Impact Analysis:** Evaluate the impact of the remaining 99-year lease period on property value.

---

## Dataset Information
**Source:** Data retrieved from [Data.gov.sg Housing Datasets](https://data.gov.sg/datasets?topics=housing&resultId=d8b84c4ee58e3cfc0ece0d773c8ca6abc)[cite: 14].

### Feature Descriptions
| Column Name | Data Type | Description |
| :--- | :--- | :--- |
| `month` | Date | The year and month when the resale transaction was registered (formatted as YYYY-MM). |
| `town` | Text | The specific HDB estate or residential town where the property is located. |
| `flat_type` | Text | The room type configuration of the HDB unit (e.g., number of rooms or executive status). |
| `block` | Text | The specific block number of the HDB building. |
| `street_name` | Text | The official street name where the HDB building is located. |
| `storey_range` | Text | The grouped floor level range where the specific unit is located. |
| `floor_area_sqm` | Numeric | The total internal floor area of the flat, measured in square meters. |
| `flat_model` | Text | The design model or architectural classification of the HDB flat. |
| `lease_commence_date` | Year | The year the 99-year lease officially began for the building. |
| `remaining_lease` | Text | The remaining duration of the 99-year lease at the time of the transaction. |
| `resale_price` | Numeric | The final agreed-upon sale price of the flat in Singapore Dollars (SGD). |

---

## Core Analytics & Key Insights

### 1. Macro Market Trends & The Pandemic Breakout
* **The Pandemic Effect:** HDB resale prices show a clear, profound structural breakout following the onset of the pandemic.
* **Market Distribution:** The vast majority of HDB flat transactions occur at affordable, entry-to-mid-tier price points.However, the market features a significant premium tier that pulls the average upward.

### 2. Location Premiums Over Raw Square Footage
* **Geography Rules:** Physical size is not the primary driver of high-end property valuation in Singapore; location completely overrides raw square footage.
***Prime vs. Suburban Case Study:** A 90 sqm 4-room flat in a non-mature, far-flung estate sits at the lower end of the valuation spectrum, while an identical 90 sqm 4-room flat located in a prime central area (like Dawson or Queenstown) shoots to the top.
* **Buyer Priorities:** Premium buyers systematically place a high financial surplus on central proximity, prestige, and top-tier schooling districts. Even within public housing, prime locations like Bukit Timah or Bishan drive median transaction costs significantly higher than their suburban equivalents.

### 3. The Vertical Premium Multiplier
* **Floor Height Impact:** Floor height acts as a major premium multiplier in Singapore's public housing sector, with buyers systematically willing to pay a progressive surplus for higher units.
* **Value Drivers:** This premium is driven by three main environmental factors: better panoramic views, reduced road and street-level noise, and superior ventilation/natural light.

### 4. Supply Dynamics & Market Liquidity
* **The Market Baseline:** 4-room units constitute the definitive "standard baseline" of Singaporean public housing, commanding a dominant 42.4% market share.
* **Bedrock Liquidity:** Flats built in the late 1970s, 1980s, and 1990s are heavily dominated by "Model A" (the highest volume model) and "Improved" architectural blueprints. Because these units represent the primary housing supply ever built across major heartland mega-towns, they form the bedrock liquidity of today's resale market.

---

## Tech Stack
* **Language:** Python 
* **Libraries:** `pandas`, `numpy` (Data Processing), `matplotlib`, `seaborn` (Data Visualization)

---

## Conclusion
This analysis successfully demonstrates that the Singapore public housing market is no longer a uniform utility.While suburban towns like Woodlands and Sengkang ensure foundational market volume and baseline affordability, a hyper-competitive layer exists where premium location models (like DBSS or high-storey central units) behave entirely like luxury assets.
