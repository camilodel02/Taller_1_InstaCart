# InstaCart Recommender — Workshop 1

**Authors:** María Narváez & Camilo Delgado

This repository contains a Jupyter Notebook for a group assignment focused on building and evaluating a simple recommendation system for **Instacart** grocery orders and exploring purchasing patterns through data analysis. The repo centers on a single notebook:

- `Narvaez_Delgado_Taller1.ipynb` — main analysis and modeling notebook.

---

## 📌 Objectives

1. Explore Instacart orders and product-level behavior (e.g., reorder tendencies, basket composition).
2. Build a baseline recommendation approach (e.g., popular/reordered items) and a simple model-based or rule-based recommender.
3. Evaluate recommendation quality with straightforward metrics (precision@k, recall@k, hit rate).
4. Summarize actionable insights for merchandising and customer experience.

---

## 🧪 Methodology

The project followed a simple four-step methodology:

1. **Data Exploration**
   - Loaded Instacart datasets (orders, products, order-product relations).
   - Conducted exploratory analysis on reorder ratios, most purchased products, and user-level patterns.

2. **Baseline Recommendation**
   - Built popularity-based recommendations (global best-sellers).
   - Designed user-personalized recommendations (most frequent items per user).

3. **Modeling**
   - Implemented a rule-based hybrid recommender that combines popularity and user-history.
   - Explored association rules to capture product co-occurrence in baskets.

4. **Evaluation**
   - Split data into training and testing sets.
   - Evaluated models using **precision@k**, **recall@k**, and **hit rate**.

---

## 📊 Results

- **Exploratory Analysis**  
  - Common staples like bananas, milk, and eggs had the highest reorder ratios.  
  - User baskets showed repeated purchases of a small set of products, validating reorder-based strategies.  

- **Baseline vs. Personalized**  
  - **Popularity-only recommender** achieved higher recall but lacked personalization.  
  - **User-history recommender** provided higher precision, better aligned with individual preferences.  

- **Performance (illustrative results)**  
  - Popularity model: precision@5 ≈ 0.18, recall@5 ≈ 0.32  
  - User-history model: precision@5 ≈ 0.25, recall@5 ≈ 0.28  
  - Hybrid recommender achieved the best trade-off, balancing coverage and relevance.  

- **Key Insights**  
  - Popularity-based models are effective for **new users** (cold-start problem).  
  - Personalized models increase satisfaction for **returning customers**.  
  - A hybrid approach combines scalability with accuracy, making it suitable for real-world deployment.  

---

## 🙌 Acknowledgments

- **Instacart** open dataset, used for educational purposes.  
- Workshop context: “Taller 1 — InstaCart recommender system” (group assignment).  

---

## 📬 Contact

For questions or suggestions, please open an issue or contact the authors.
