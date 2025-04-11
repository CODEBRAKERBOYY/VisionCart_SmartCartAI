# 🛒 SmartCart-AI: Multi-Agent System for Personalized E-Commerce

## 📌 Challenge Overview

In the competitive world of e-commerce, delivering personalized and relevant product recommendations is critical to improving customer experience, increasing conversion rates, and boosting sales.

**SmartCart-AI** is a multi-agent AI system designed to generate hyper-personalized product recommendations by leveraging:

- Customer behavior
- Product metadata
- Sentiment scores
- Seasonality and shopping patterns

This project was developed for **"Hack the Future: GenAI Sprint – Smart Shopping Challenge"**.

---

## 🧠 Architecture Overview

SmartCart-AI consists of **three core agents**, each performing a specific role:

| Agent               | Function                                                                 |
|--------------------|--------------------------------------------------------------------------|
| 👤 Customer Agent   | Tracks user demographics, browsing behavior, and purchase history         |
| 📦 Product Agent    | Manages product metadata, pricing, availability, sentiment & seasonality |
| 🧠 Recommendation Agent | Uses a hybrid AI model (content-based + rule scoring) to generate top-N product recommendations |

All agent outputs are saved in a **SQLite database** for long-term memory and future use.

---

## 🗃️ Dataset

Located in the `/data` folder:

- `customer_data_collection.csv` – Contains user demographics, browsing and purchase history
- `product_recommendation_data.csv` – Contains product metadata, ratings, seasonality, and sentiment

---

## 💾 Long-Term Memory with SQLite

The `/database` folder contains:

- `smartcart.db` – SQLite database with:
  - `customer_profiles` table
  - `product_profiles` table
  - `recommendations` table (final output)

---

## 📂 Project Structure

