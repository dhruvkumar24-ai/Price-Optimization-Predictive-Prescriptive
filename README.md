# 🥑 Price Optimization using Predictive & Prescriptive Analytics
### Regression · MILP · Gurobi · Scikit-learn · Python · OR Course Project

![Python](https://img.shields.io/badge/Python-3.11+-3776AB?style=flat-square&logo=python&logoColor=white)
![Gurobi](https://img.shields.io/badge/Gurobi-Optimizer-red?style=flat-square)
![Sklearn](https://img.shields.io/badge/Scikit--learn-Regression-F7931E?style=flat-square&logo=scikit-learn&logoColor=white)
![Status](https://img.shields.io/badge/Status-Optimal_Revenue_Found-brightgreen?style=flat-square)
![Course](https://img.shields.io/badge/IIT_Kanpur-Data_Mining_Course_Project-red?style=flat-square)

---

## 🧩 Problem Statement

As a supplier, setting avocado prices requires a delicate trade-off — too high and you lose customers, too low and you lose profit. This project builds a **full data science pipeline** that answers:

> *"What is the optimal price and supply quantity for avocados across 8 US regions to maximize net revenue, accounting for demand elasticity, wastage, and transportation costs?"*

**Data:** Real sales data (2015–2022) from the [Hass Avocado Board](https://hassavocadoboard.com/) — 6,804 rows across 8 US regions.

---

## ⚙️ Three-Stage Analytics Pipeline

```
Stage 1: DESCRIPTIVE
        │
        ├── EDA: price trends, regional demand, seasonality
        └── Correlation analysis across regions & years
        │
        ▼
Stage 2: PREDICTIVE
        │
        ├── Regression model: Demand = f(price, region, year, seasonality)
        └── R² ≈ 0.90 — captures price elasticity & regional variation
        │
        ▼
Stage 3: PRESCRIPTIVE
        │
        ├── Non-convex MILP in Gurobi
        ├── Objective: Maximize revenue - wastage cost - transport cost
        └── Output: Optimal price & allocation per region
```

---

## 📊 Key Results

| Metric | Value |
|---|---|
| **Optimal Net Revenue** | **$33.09M** |
| **Demand Model R²** | **≈ 0.90** |
| **Revenue Improvement** | **~35% vs. historical benchmarks** |
| **Regions Optimized** | 8 US regions |
| **Data Points** | 6,804 rows (2015–2022) |

**Optimal Pricing by Region:**

| Region | Actual Price | Optimal Price |
|---|---|---|
| West | $0.83 | $2.00 |
| SouthCentral | $0.65 | $1.92 |
| Northeast | $1.04 | $1.90 |
| Southeast | $0.82 | $1.66 |
| Great Lakes | $0.80 | $1.53 |

---

## 🔑 Model Highlights

| Component | Detail |
|---|---|
| **Predictive Model** | Regression (price elasticity + seasonality + region) |
| **Prescriptive Model** | Non-convex MILP via Gurobi |
| **Objective** | Maximize revenue − wastage − transportation cost |
| **Constraints** | Supply limits, demand satisfaction, allocation bounds |
| **Zero Wastage** | Optimal solution achieves zero wastage across all regions |

---

## 📁 Repository Structure

```
📦 Price-Optimization-Predictive-Prescriptive/
├── Price_Optimization_Avocado_Gurobi.ipynb   # Full pipeline: EDA + regression + MILP
├── README.md
└── LICENSE
```

---

## 🚀 Getting Started

```bash
pip install gurobipy pandas numpy scikit-learn matplotlib seaborn
```

> Gurobi Academic License required. Available free via [Gurobi Academic Program](https://www.gurobi.com/academia/academic-program-and-licenses/).

Open `Price_Optimization_Avocado_Gurobi.ipynb` — all outputs and visualizations are pre-computed.

---

## 🧠 Concepts Covered

`Price Elasticity` · `Demand Forecasting` · `Descriptive Analytics` · `Predictive Modelling` · `Prescriptive Analytics` · `Non-convex Optimization` · `MILP` · `Revenue Maximization` · `Supply Chain`

---

## 📚 Reference

Gurobi Modeling Examples — [Price Optimization](https://github.com/Gurobi/modeling-examples/tree/master/price_optimization)

---

## 👤 Author

**Dhruv Kumar Sahu**
M.Tech, Industrial & Management Engineering — IIT Kanpur
GATE 2024 AIR 33 | [LinkedIn](https://www.linkedin.com/in/dhruv-kumar-sahu-157ab9193/) · [GitHub](https://github.com/dhruvkumar24-ai)
