<div align="center">

# <h1> Hotel Management Data Analysis

</div>

<p align="center">
  <img src="https://img.shields.io/badge/Data%20Analytics-EDA-blue?style=for-the-badge"/>
  <img src="https://img.shields.io/badge/Hotel%20Analytics-Revenue%20%26%20Cancellations-orange?style=for-the-badge"/>
  <img src="https://img.shields.io/badge/Customer%20Segmentation-ML-green?style=for-the-badge"/>
</p>

<p align="center">
A data-driven study of booking patterns, customer behavior, cancellation risks, and hotel revenue performance.
</p>


---


# Project Overview

This project provides a complete analysis of hotel booking data with the goal of uncovering:

Cancellation patterns and risk factors

ADR (Average Daily Rate) and revenue insights

Customer segmentation

Market, country, and distribution channel behavior

Data-backed business recommendations


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

1. Cancellation Behavior

Overall cancellation rate: 37.04%

City Hotel cancellation rate: 41.7%

Resort Hotel cancellation rate: 27.8%
City hotels experience significantly higher demand volatility.


2. ADR (Average Daily Rate) Insights

Overall ADR: ₹101.83

City Hotel ADR: ₹105.30

Resort Hotel ADR: ₹94.95

City Hotels earn roughly ₹10.35 more per night on average.


3. Higher ADR → Higher Cancellation Risk

Booking Type	ADR

Canceled	₹104.96
Not Canceled	₹99.99


Canceled bookings are, on average, ₹4.97 higher in ADR.

4. Country-Level Insights (Top 5 by volume)

Country Code	Country	Bookings

PRT	Portugal	48,590
GBR	United Kingdom	12,129
FRA	France	10,415
ESP	Spain	8,568
DEU	Germany	7,287


Portugal represents the largest segment of total bookings.

5. Distribution Channels & Agents

Majority of reservations come via online travel agencies (OTAs).

Direct bookings are fewer but more reliable.

Certain agents contribute a disproportionate share of bookings and revenue.


6. Customer Segmentation (K-Means + Rules)

Four clear clusters emerged:

Cluster	Segment Description

0	Budget last-minute travelers
1	High-value planners (high ADR + long lead time)
2	Families / group travelers
3	Vacation travelers (long stays, mid-high ADR)

---

# Analysis Modules Included

1. Cancellation Analysis

Lead time, deposit status, distribution channel, country, booking history, and model-based predictors.

2. ADR & Revenue Analysis

ADR trends by hotel type, country, channel, and customer segment.
Revenue estimation using nights stayed.

3. Customer Segmentation

Rule-based segmentation and K-Means clustering with profiling.

4. Distribution Channel & Agent Performance

Booking volume, cancellation characteristics, ADR contribution, revenue share.

5. Country-Wise Analysis

Booking count, cancellation rate, ADR, revenue, and stay duration by country.


---


# Business Recommendations

### 1. Improve Overbooking Strategy

High cancellation rates justify controlled overbooking, especially in City Hotels.
Prediction-based overbooking can minimize lost revenue.

### 2. Strengthen Direct Booking Programs

Direct bookings deliver:

Lower cancellations

Lower acquisition cost

Higher guest lifetime value
Promote loyalty points, flexible benefits, and targeted offers.


### 3. Dynamic Pricing by Customer Segment

High-value planners → premium packages

Families → bundled offerings

Last-minute travelers → tactical pricing


### 4. Focus Marketing on High-Value Countries

Countries with high ADR and revenue potential should be prioritized.

### 5. Monitor Agent & OTA Performance

Analyze agent-level contribution to revenue, cancellations, and profitability.
Negotiate better terms for low-performing, high-cancellation channels.


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
