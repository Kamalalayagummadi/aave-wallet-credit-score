# 🛡️ Wallet Risk Scoring from On-Chain Activity

## 📌 Problem Statement

Given a list of 100 wallet addresses, this project:
- Fetches their Compound V2 on-chain transactions
- Engineers relevant features to reflect wallet risk
- Scores each wallet on a scale from **0 (high risk)** to **1000 (low risk)**

## ✅ Tasks Completed

1. **Transaction Data Collection** using Covalent API  
2. **Feature Engineering**  
   - Transaction count
   - Total ETH transferred
   - Number of successful txs
   - Average gas price
   - Inbound vs outbound transfers
   - Days since last tx
3. **Risk Score Generation**
   - Feature normalization
   - Weighted scoring logic
4. **Final Output CSV** with `wallet_id` and `score`

## 📁 Files

| File                          | Description                           |
|-------------------------------|---------------------------------------|
| `wallet_risk_scoring.ipynb`   | Full notebook code                    |
| `final_wallet_risk_scores.csv`| Final output for submission           |
| `requirements.txt`            | Required Python packages              |
| `explanation.md`              | Detailed method explanation           |
