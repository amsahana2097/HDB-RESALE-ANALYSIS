# Singapore HDB Resale Trend Analysis Using Python

## Project Overview
[cite_start]This repository contains an exploratory data analysis (EDA) and visualization project focused on the Singapore Housing & Development Board (HDB) resale property market[cite: 1, 10]. [cite_start]The analysis bridges raw historical property records with data visualization techniques to uncover trends, price growth trajectories, and structural relationships within the housing market[cite: 10, 11, 235].

[cite_start]Historically viewed as uniform public housing utilities, the Singapore public housing market has evolved to behave like a mature, competitive asset class with distinct foundational and luxury-tier segments[cite: 236, 237].

---

## Project Objectives
* [cite_start]**Track Town Trajectories:** Monitor and track town-by-town price growth trajectories across Singapore[cite: 3].
* [cite_start]**Property Valuation Dynamics:** Analyze how property valuations scale over the years[cite: 4].
* [cite_start]**Quantify Resale Price Index:** Analyze the resale price index to quantify market movements[cite: 5].
* [cite_start]**Assess Structural Influences:** Evaluate how flat types, architectural models, and physical size influence final resale prices[cite: 6, 8].
* [cite_start]**Lease Impact Analysis:** Evaluate the impact of the remaining 99-year lease period on property value[cite: 7].

---

## Dataset Information
* [cite_start]**Source:** Data retrieved from [Data.gov.sg Housing Datasets](https://data.gov.sg/datasets?topics=housing&resultId=d8b84c4ee58e3cfc0ece0d773c8ca6abc)[cite: 14].

### Feature Descriptions
| Column Name | Data Type | Description |
| :--- | :--- | :--- |
| `month` | Date | [cite_start]The year and month when the resale transaction was registered (formatted as YYYY-MM)[cite: 16]. |
| `town` | Text | [cite_start]The specific HDB estate or residential town where the property is located[cite: 16]. |
| `flat_type` | Text | [cite_start]The room type configuration of the HDB unit (e.g., number of rooms or executive status)[cite: 16]. |
| `block` | Text | [cite_start]The specific block number of the HDB building[cite: 16]. |
| `street_name` | Text | [cite_start]The official street name where the HDB building is located[cite: 16]. |
| `storey_range` | Text | [cite_start]The grouped floor level range where the specific unit is located[cite: 16]. |
| `floor_area_sqm` | Numeric | [cite_start]The total internal floor area of the flat, measured in square meters[cite: 16]. |
| `flat_model` | Text | [cite_start]The design model or architectural classification of the HDB flat[cite: 18]. |
| `lease_commence_date` | Year | [cite_start]The year the 99-year lease officially began for the building[cite: 18]. |
| `remaining_lease` | Text | [cite_start]The remaining duration of the 99-year lease at the time of the transaction[cite: 18]. |
| `resale_price` | Numeric | [cite_start]The final agreed-upon sale price of the flat in Singapore Dollars (SGD)[cite: 18]. |

---

## Core Analytics & Key Insights

### 1. Macro Market Trends & The Pandemic Breakout
* [cite_start]**The Pandemic Effect:** HDB resale prices show a clear, profound structural breakout following the onset of the pandemic[cite: 218].
* [cite_start]**Market Distribution:** The vast majority of HDB flat transactions occur at affordable, entry-to-mid-tier price points[cite: 219]. [cite_start]However, the market features a significant premium tier that pulls the average upward[cite: 220].

### 2. Location Premiums Over Raw Square Footage
* [cite_start]**Geography Rules:** Physical size is not the primary driver of high-end property valuation in Singapore; location completely overrides raw square footage[cite: 225, 227].
* [cite_start]**Prime vs. Suburban Case Study:** A 90 sqm 4-room flat in a non-mature, far-flung estate sits at the lower end of the valuation spectrum, while an identical 90 sqm 4-room flat located in a prime central area (like Dawson or Queenstown) shoots to the top[cite: 226].
* [cite_start]**Buyer Priorities:** Premium buyers systematically place a high financial surplus on central proximity, prestige, and top-tier schooling districts[cite: 221]. [cite_start]Even within public housing, prime locations like Bukit Timah or Bishan drive median transaction costs significantly higher than their suburban equivalents[cite: 222, 224].

### 3. The Vertical Premium Multiplier
* [cite_start]**Floor Height Impact:** Floor height acts as a major premium multiplier in Singapore's public housing sector, with buyers systematically willing to pay a progressive surplus for higher units[cite: 228, 229].
* [cite_start]**Value Drivers:** This premium is driven by three main environmental factors: better panoramic views, reduced road and street-level noise, and superior ventilation/natural light[cite: 230].

### 4. Supply Dynamics & Market Liquidity
* [cite_start]**The Market Baseline:** 4-room units constitute the definitive "standard baseline" of Singaporean public housing, commanding a dominant 42.4% market share[cite: 231].
* [cite_start]**Bedrock Liquidity:** Flats built in the late 1970s, 1980s, and 1990s are heavily dominated by "Model A" (the highest volume model) and "Improved" architectural blueprints[cite: 232]. [cite_start]Because these units represent the primary housing supply ever built across major heartland mega-towns, they form the bedrock liquidity of today's resale market[cite: 233].

---

## Tech Stack
* [cite_start]**Language:** Python [cite: 1]
* **Libraries:** `pandas`, `numpy` (Data Processing), `matplotlib`, `seaborn` (Data Visualization)

---

## Conclusion
[cite_start]This analysis successfully demonstrates that the Singapore public housing market is no longer a uniform utility[cite: 235, 236]. [cite_start]While suburban towns like Woodlands and Sengkang ensure foundational market volume and baseline affordability, a hyper-competitive layer exists where premium location models (like DBSS or high-storey central units) behave entirely like luxury assets[cite: 237].