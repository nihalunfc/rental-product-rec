# Rental Product Recommendation System (Kaggle)

## Project Overview
This project is for the Kaggle "Rental Product Recommendation System" competition. The goal is to predict the next product a user will visit in a session-based browsing environment for a children’s product rental marketplace.

**Objective:** Predict exactly 6 `product_id` values for each `visit_id` using **Recall@6** as the evaluation metric.

## Prerequisite Knowledge
* **Session-Based Recommendations:** Understanding user intent within a single browsing window.
* **Candidate Generation:** Using Co-visitation matrices and "Frequently Viewed Together" logic.
* **Ranking Models:** Implementing LightGBM/XGBoost to rank potential product candidates.
* **Cold Start Strategy:** Handling new products using metadata-based similarity.

## Current Setup & Progress
- [ ] Initialize Repository
- [ ] Data Exploration (EDA)
- [ ] Baseline Model (Top 6 Popular Items)
- [ ] Feature Engineering (Session length, Category affinity)
- [ ] Final Submission Script (Offline compliant)

## How to Run
1. Clone the repo: `git clone <your-repo-link>`
2. Place Kaggle data in the `/data` folder.
3. Run the baseline notebook: `notebooks/01_baseline_popularity.ipynb`

## Important Note
This competition requires **offline inference**. All models and lookup tables are stored in the `/models` directory to ensure no internet access is required during prediction.
