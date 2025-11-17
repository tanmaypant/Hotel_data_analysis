# 🏨 Hotel Management Data Analysis
Unlocking insights from booking patterns, customer behavior & hotel revenue data
<p align="center"> <img src="https://img.shields.io/badge/Data%20Science-EDA-blue?style=for-the-badge"/> <img src="https://img.shields.io/badge/Hotel%20Analytics-Revenue%20%26%20Cancellations-orange?style=for-the-badge"/> <img src="https://img.shields.io/badge/Customer%20Segmentation-ML-green?style=for-the-badge"/> </p>

---

# 📘 Project Overview

This project performs an end-to-end data analysis on hotel booking data to uncover:

✔ Cancellation patterns & risk drivers

✔ ADR & revenue performance

✔ Customer segmentation

✔ Market, country & channel insights

✔ Business recommendations for hotel operations

Using Python-based exploratory data analysis (EDA), clustering, and performance metrics, this project gives hotels actionable intelligence to improve revenue, reduce cancellations, and optimize distribution strategies.
 
---

# 🛠️ Tech Stack

- **Python (Pandas, NumPy)** — Data manipulation & preprocessing  
- **Matplotlib, Seaborn** — Visualization  
- **Scikit-Learn** — Machine learning & clustering  
- **Jupyter Notebook** — Interactive analysis  
- **GitHub** — Version control & documentation

---

# 📁 Dataset Overview

The dataset contains 36 columns and hundreds of thousands of bookings, covering:

🏨 Hotel type (City / Resort)

📅 Arrival dates (year, month, week number)

👨‍👩‍👧 Guests (adults, children, babies)

💰 ADR (Average Daily Rate)

🚗 Special requests & parking

📦 Market segment & distribution channel

🌍 Country of origin

🔁 Previous cancellations

📄 Reservation status

💳 Deposit & payment behavior

---

From this dataset, several new features were engineered:

total_nights = weekday + weekend nights

revenue = adr × total_nights

family_size = adults + children + babies

customer_group (Solo / Couple / Family)

value_segment (Low / Mid / High ADR tiers)

🔢 Key Findings (Summary of Real Calculations)
📉 1. High Cancellation Rate

Overall cancellation rate: 37.04%

City Hotel cancellations: 41.7%

Resort Hotel cancellations: 27.8%

📌 City hotels face much higher volatility in demand.

💵 2. ADR Insights

Overall ADR: ₹101.83

City Hotel ADR: ₹105.30

Resort Hotel ADR: ₹94.95

Difference: City hotels charge ₹10.35 more per night

📌 City hotels earn more per night but also see more cancellations.

❌ 3. Higher ADR → Higher Cancellation Risk
Booking Type	ADR
Canceled	₹104.96
Not Canceled	₹99.99

📌 Canceled bookings have ₹4.97 higher ADR on average.

🌍 4. Top Countries by Booking Volume
Country	Full Name	Bookings
PRT	Portugal	48,590
GBR	United Kingdom	12,129
FRA	France	10,415
ESP	Spain	8,568
DEU	Germany	7,287

📌 Portugal dominates due to local tourism & OTA exposure.

📊 5. Distribution Channels & Agents

Most bookings come through Online Travel Agencies (OTA / TA/TO)

Direct bookings account for fewer reservations but generally higher reliability

Certain agents dominate both booking volume & revenue

📌 Channel and agent management has high financial impact.

🧩 6. Customer Segmentation (K-Means + Rules-Based)

The project identifies 4 clear customer clusters:

Cluster	Description
0	Budget last-minute travelers
1	High-value planners (high ADR + long lead times)
2	Family/group travelers
3	Vacation travelers (long stays, mid-high ADR)

📌 Segmentation helps in targeted marketing and personalized offers.

🧪 Analysis Modules Included
✔ 1. Cancellation Analysis

Lead time effect

Market, channel & country influence

Deposit impact

Predictive features & model

Outlier filtering

✔ 2. ADR & Revenue Analysis

ADR by hotel, country, month, channel

Revenue calculations

High-value customer identification

Performance benchmarking

✔ 3. Customer Segmentation

Rule-based (family size, stay length, ADR tiers)

K-Means clustering

Cluster profiling

✔ 4. Distribution & Agent Analysis

Booking share

ADR & revenue by channel

Agent contribution analysis

✔ 5. Country-Wise Performance

Booking count

Cancellation rate

ADR ranking

Revenue ranking

Stay duration

---

# 💡 Business Recommendations
🔹 1. Optimize Overbooking Strategy

Given a 37% cancellation rate, hotels should:

Apply higher overbooking buffers for City Hotels

Use cancellation prediction scores to guide overbooking

🔹 2. Strengthen Direct Booking Incentives

Direct bookings have:

Lower cancellations

Lower commissions

Higher lifetime value

Offer:

Loyalty points

Early check-in

Free room upgrades

🔹 3. Dynamic Pricing by Segment

High-value planners (Cluster 1) → premium packages

Families (Cluster 2) → bundle deals (parking, meals)

Last-minute travelers (Cluster 0) → targeted discounts

🔹 4. Market Focus on High-Value Countries

Countries with higher ADR & revenue should be targeted with tailored ad campaigns.

🔹 5. Agent & OTA Monitoring

Identify top-performing agents (high revenue, low cancellations).
Re-negotiate commissions with low-value/high-cancellation agents.

---

# 📞 Contact

For collaboration, improvements, or reporting support
Author: Tanmay

Email: panttanmay20@gmail.com

LinkedIn: [tanmaypant](https://www.linkedin.com/in/tanmay-pant-4916102a9)

---

# 🏁 Conclusion

This project demonstrates how raw hotel booking data can be transformed into meaningful insights using data analytics and machine learning.
It supports better decisions in:

Revenue management

Marketing

Customer personalization

Channel optimization

Operational planning

✨ Feel free to fork, star ⭐, or contribute to this repository!
