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

### 1. Adjust Overbooking Based on Risk

City Hotels have a 41.7% cancellation rate, and guests with 0 special requests cancel nearly 48% of the time.
By overbooking more in these high-risk segments—and less for low-risk guests (4–5 requests → only 5–11% cancellations)—hotels can reduce empty rooms and recover lost revenue.

### 2. Shift More Bookings Toward Direct Channels

Online Travel Agencies (OTAs) dominate bookings but also correlate with higher last-minute cancellations.
Direct bookings have lower cancellation behavior and avoid OTA commissions, meaning even a 5–10% shift toward direct channels can increase net revenue without raising prices.

### 3. Create Targeted Offers for Each Customer Segment

Couples form the majority of bookings (over 55–60%), so couple-specific deals can increase conversion.
Families stay longer, meaning even fewer bookings can generate more total revenue.
Solo travelers—often business guests—benefit from weekday discounts, helping raise occupancy during low-demand days.

### 4. Use Pricing Strategies Based on ADR Patterns

Transient guests have the highest ADR (₹107), while groups and contracts are much lower (₹83–87).
Using dynamic pricing—especially for high-ADR segments—can increase room revenue.
Canceled bookings also have ₹4.97 higher ADR, signaling potential overpricing; offering partial prepaid rates or small flexibility incentives can reduce this.

### 5. Focus Marketing on High-Value Countries

Portugal alone provides 48,590 bookings, and Western Europe (UK, France, Spain, Germany) adds tens of thousands more.
Targeting these stable, high-volume regions ensures better ROI.
High-ADR markets like Djibouti (₹275+) and Anguilla (₹265) should be targeted with premium packages.
High-cancellation regions (ARE, SAU, IDN at 68–84%) should face stricter policies to protect revenue.

### 6. Build Packages Around Popular Stay Lengths

Short stays (2–3 nights) dominate overall demand.
Medium stays (4–7 nights) are typically vacation-oriented and drive higher ADR, especially for Resort Hotels.
Long stays (8+ nights) are rare but produce the highest total revenue per booking, making them ideal for extended-stay promotions and corporate tie-ups.

### 7. Use Special Requests to Predict Commitment

Guests with 0 requests cancel heavily (48%), while those with 4–5 requests almost never cancel (5–11%).
Encouraging guests to add preferences during booking (meal type, bed type, parking, etc.) increases engagement and reduces cancellation probability, improving occupancy stability.


---


# Contact

Author: Tanmay
Email: panttanmay20@gmail.com
LinkedIn: tanmaypant


---


# Conclusion

This project demonstrates how hotel booking data can be transformed into useful insights that support:

Revenue management

Operational planning

Customer segmentation

Marketing strategy

Cancellation risk reduction


Feel free to fork, star ⭐, or open an issue for improvements.


---
