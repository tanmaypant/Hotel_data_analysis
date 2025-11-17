# Hotel Management Data Analysis

  <img src="https://img.shields.io/badge/Data%20Analytics-EDA-blue?style=for-the-badge"/>
  <img src="https://img.shields.io/badge/Hotel%20Analytics-Revenue%20%26%20Cancellations-orange?style=for-the-badge"/>

A data-driven study of booking patterns, customer behavior, cancellation risks, and hotel revenue performance.


---


# Project Overview

This project provides a complete analysis of hotel booking data with the goal of uncovering:

- Cancellation patterns and risk factors

- ADR (Average Daily Rate) and revenue insights

- Customer segmentation

- Market, country, and distribution channel behavior

- Data-backed business recommendations


Through exploratory data analysis (EDA), clustering techniques, and statistical profiling, this study offers actionable insights to help hotels improve revenue, reduce cancellations, and optimize operational strategy.


---


# Tech Stack

- Python (Pandas, NumPy) — Data preparation and manipulation

- Matplotlib, Seaborn — Visualization and trend analysis

- Scikit-Learn — Machine learning & clustering

- Jupyter Notebook — Interactive development environment

- GitHub — Version control and documentation


---


# Dataset Overview

The dataset includes 36+ attributes covering:

- Hotel type (City / Resort)

- Arrival date details

- Guest composition

- ADR (Average Daily Rate)

- Special requests and parking

- Market segment & distribution channel

- Country of origin

- Cancellation indicators

- Booking lead time

- Deposit status


---


# Key Findings

### Cancellation Analysis

 Overall cancellation rate: 37.04%
 - About 37% of all hotel bookings are canceled.

<img width="577" height="457" alt="image" src="https://github.com/user-attachments/assets/d2be3258-fe6a-45eb-8191-45fc4c7044db" />

City Hotel cancellation rate: 41.7%
Resort Hotel cancellation rate: 27.8%
- City Hotels have MUCH higher cancellation rate than Resort Hotels.
- People often book City Hotels for business/work → higher last-minute changes.
- Resort bookings are usually planned vacations → much lower cancellation.

<img width="568" height="457" alt="image" src="https://github.com/user-attachments/assets/37208ecf-fdd8-443d-bd2d-a271a66f00b2" />

- Guests with 0 special requests have the highest cancellation rate (~48%)
- Cancellation rate drops significantly once a guest makes even 1 request -> From ~48% → ~22%
- Guests with 2–3 special requests remain stable (~18–22% cancellation rate)
- Special requests of 4 or more show extremely low cancellation
  - 4 requests → ~11%
  - 5 requests → ~5%

### ADR (Average Daily Rate) Insights

Overall ADR: ₹101.83
City Hotel ADR: ₹105.30
Resort Hotel ADR: ₹94.95
- City Hotels charge ~₹10.35 more per night than Resort Hotels.
- This is a +10.9% difference.

ADR by customer type

| Customer Type   | ADR (Average Daily Rate) |
| --------------- | ------------------------ |
| Contract        | 87.55                    |
| Group           | 83.49                    |
| Transient       | 107.01                   |
| Transient-Party | 86.08                    |

- Transient customers have the highest ADR at ~107
- Group ADR is the lowest (~83.49).
- Contract customers (~87.55) have fixed negotiated rates.
- Transient-Party ADR (~86.08) is slightly below Contract and much below pure Transient.

Booking Type ADR

<img width="695" height="452" alt="image" src="https://github.com/user-attachments/assets/8104e123-82de-4215-adaf-fdbb1216b99b" />

Canceled	₹104.96
Not Canceled	₹99.99
- Canceled bookings are, on average, ₹4.97 higher in ADR.

### Customer Segmentation

Segmentation based on guest 

<img width="790" height="490" alt="image" src="https://github.com/user-attachments/assets/1cb0e5f7-b010-46e5-8330-8d3e3d82c6ab" />

- Couples dominate (≈ 55–65% of bookings)
- Families are the second largest
- Solo travelers are least common

Segmentation based on market type 

<img width="989" height="490" alt="image" src="https://github.com/user-attachments/assets/02f84463-9841-4ff7-99f3-2b8a426d504f" />

- Online Travel Agencies (OTA) usually dominate (40–60%)
- Direct bookings take 15–25
- Corporate 10–20%
- Groups lower volume but longer stays

Segmentation based on length of stay

<img width="889" height="489" alt="image" src="https://github.com/user-attachments/assets/24e34b32-9fc6-40cd-b905-fef5c8de820c" />

- Majority of bookings are usually short stays (2–3 nights)
- Long stays (8+ nights) are rare but generate high ADR
- “Medium stays” (4–7 nights) are typical for vacations (resort hotel bookings)

### Country-Level Insights (Top 5 by volume)

Top 5 countries 

<img width="1025" height="549" alt="image" src="https://github.com/user-attachments/assets/5ea3b81a-071b-4c73-9cc1-30e35045fe74" />

- Portugal (PRT) overwhelmingly leads with the highest booking count, contributing nearly 4× more bookings than any other country.
- United Kingdom, France, Spain, and Germany form a strong international customer base, showing heavy Western European travel influence.
- Demand is heavily domestic + Western European, indicating where hotels should focus marketing and seasonal pricing strategies.

Cancellation Rate by Country

<img width="851" height="472" alt="image" src="https://github.com/user-attachments/assets/fba5ae80-6e72-4d37-8c8b-490b285c5ee0" />

- United Arab Emirates (ARE) has an extremely high cancellation rate (~84%), indicating very uncertain or last-minute booking behavior.
- Saudi Arabia (SAU) and Indonesia (IDN) also show high cancellation rates (~69%), suggesting weaker booking commitment from these markets.
- Philippines (PHL) and Nigeria (NGA) have cancellation rates above 60%, making them high-risk regions where stricter payment policies or confirmation steps may be needed.

ADR by Country

<img width="1006" height="549" alt="image" src="https://github.com/user-attachments/assets/83c34358-80c1-4830-80e9-64993d417fce" />

- Djibouti (DJI) has the highest ADR (~₹275), indicating premium-priced bookings—likely due to limited supply or luxury-oriented stays.
- Anguilla (AIA) and Andorra (AND) also show very high ADR values (₹200–₹265 range), suggesting strong demand from high-spending travelers.
- UMI and LAO maintain ADRs above ₹180, indicating that guests from these countries consistently book higher-priced rooms compared to average international travelers.


---


# Business Recommendations

### 1.  Implement Risk-Adjusted Overbooking Policies
The Opportunity: Our current cancellation data justifies a higher overbooking buffer for specific segments.

Key Insight: City Hotels cancel 41.7% of bookings, and zero-request guests cancel 48%. These high-risk segments should have higher overbooking allowances.

Mitigation: Crucially, low-risk guests (4–5 requests, only 5–11% cancellation rate) should not be overbooked to safeguard our service reputation and avoid costly service failures.

### 2.  Accelerate Direct Booking Acquisition
The Challenge: Online Travel Agencies (OTAs) drive high volume but are also associated with high cancellations and significant commission leakage.

Strategic Goal: Shift even a small share of volume from OTAs to our direct channels.

The Impact: This move will immediately increase net revenue per booking and concurrently reduce booking volatility and reliance on third-party channels.

### 3.  Tailor Offers to Targeted Customer Segments
Data Highlight: Couples account for 55–60% of all bookings. This is our largest single demographic.

Action: Launch highly targeted couple packages.

Further Segmentation: Develop personalized deals for Families (who drive longer stays) and Solo/Business guests (who are ideal for filling crucial mid-week occupancy).

### 4.  Leverage ADR Insights for Dynamic Pricing
The Disparity: Transient guests command the highest Average Daily Rate (ADR) at ₹107, while Groups and Contracts pay significantly less (₹83–₹87).

Strategy: Implement a more sophisticated dynamic pricing model to maximize yield from the high-paying transient segment.

Cancellation Reduction: Consider offering prepaid or non-refundable discounts, as canceled bookings currently show a higher ADR of ₹4.97, indicating we are losing high-value reservations.

### 5.  Focus Marketing on High-Value Source Countries
Current Performance: Portugal and Western European markets are the current volume drivers.

New Target: Direct premium marketing efforts towards high-ADR countries like DJI and AIA (>₹250 ADR).

ROI Focus: By targeting these segments, we ensure our marketing spend is focused on markets that generate the highest revenue per available room.

### 6.  Create Packages to Drive Extended Stay Duration
The Goal: Improve occupancy stability and increase Total Revenue per Customer.

Key Finding: While short stays dominate volume, medium (4–7 nights) and long stays generate significantly higher total revenue.

Initiative: Roll out compelling 5+ night packages and extended-stay deals to shift the mix towards more profitable, longer reservations.

### 7.  Utilize Special Requests as a Commitment Indicator
The Correlation: There is a clear, inverse relationship between the number of special requests and cancellation risk. Zero-request bookings cancel almost half the time.

The Insight: Bookings with 4–5 requests show less than an 11% cancellation rate, indicating higher commitment.

Actionable Step: Implement a smoother, more proactive flow in our direct booking process to encourage guests to add preferences, serving as a soft-commitment mechanism to reduce overall cancellation risk.

---


# Contact

Author: Tanmay
Email: panttanmay20@gmail.com
LinkedIn: [tanmaypant](https://www.linkedin.com/in/tanmay-pant-4916102a9/)


---


Feel free to fork, star ⭐, or open an issue for improvements.
