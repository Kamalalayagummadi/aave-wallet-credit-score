# Aave V2 Wallet Credit Scoring

This project assigns a credit score (0–1000) to each wallet based on its transaction behavior on the Aave V2 protocol using DeFi transaction data.

## 🚀 Overview

Each wallet interacts through actions such as:
- `deposit`
- `borrow`
- `repay`
- `redeemunderlying`
- `liquidationcall`

We analyze these patterns and score them for creditworthiness.

## 🔍 Steps Followed

1. Loaded and parsed JSON transaction data.
2. Engineered features: deposit/borrow/repay counts, totals, active days.
3. Applied a custom scoring function based on user activity.
4. Generated `wallet_scores.json`.
5. Plotted wallet score distribution as `score_distribution.png`.

## 📦 Output Files

- `wallet_scores.json` – Scores for each wallet
- `score_distribution.png` – Histogram of credit scores

## 💡 How to Run

Open `score_runner.ipynb` or `score_runner.py` and run all cells.

## 📬 Author

Kamalalaya Gummadi
