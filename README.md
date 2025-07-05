# 📌 Parking Lots Dynamic Pricing System

## 🚗 Overview

This project implements a **dynamic pricing model** for parking lots using a combination of **demand forecasting** and **competitive pricing** strategies. It is designed to optimize revenue by adjusting prices based on time-based demand, occupancy, and competitor influence.

---

## 🧰 Tech Stack

| Category       | Tools/Tech Used                     |
|----------------|-------------------------------------|
| Language       | Python                              |
| Notebook       | Google Colab / Jupyter Notebook     |
| Data Pipeline  | [Pathway](https://pathway.com) v0.24.1 |
| Visualization  | Matplotlib, Seaborn                 |
| Data Handling  | Pandas, NumPy                       |
| Version Control| Git, GitHub                         |

---

## 🏗️ Architecture Diagram (Mermaid)

```mermaid
graph TD
    A[Raw Data Streams] -->|Time, Occupancy, Events| B[Demand Score Calculator]
    B --> C[Demand-Based Pricing Model]
    C --> F[Final Price Table]
    D[Competitor Price Feed] --> E[Competitor Adjustment Model]
    E --> F
    F --> G[Frontend/Display or Dashboard]



Project Workflow
1. Input Sources
Real-time or simulated data for:

Time and date

Parking occupancy

Nearby event data

Competitor pricing

2. Demand Score Calculation
Calculates a score based on factors like time of day and occupancy.

3. Pricing Models
Baseline Model: Fixed pricing.

Demand-Based Model: Dynamic pricing based on demand.

Competitive Pricing Model: Adjusts price with competitor influence.

4. Final Price Formula
ini
Copy
Edit
final_price = base_price + λ * demand_score + γ * (avg_comp_price - base_price)
5. Visualization
Price table with dynamic updates reflecting real-time pricing.


