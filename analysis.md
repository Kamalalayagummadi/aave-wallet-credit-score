# Credit Score Analysis – Aave V2

We analyzed the behavior of 100,000 DeFi wallet transactions and scored 50,000+ unique wallets.

# 📊 Score Distribution

| Score Range | Wallet Count | Behavior Summary                         |
|-------------|--------------|------------------------------------------|
| 0–99        | Very few      | Liquidated or highly risky behavior      |
| 100–300     | Low           | Mostly borrowed but didn't repay        |
| 400–600     | Moderate      | Some repayment, not frequent             |
| 600–800     | High          | Consistent deposits, repays, few risks   |
| 800–1000    | Excellent     | High activity, responsible users         |

# 🧠 Observations

- Wallets with high deposits and repayments consistently scored above 800.
- Wallets with many borrow actions and zero repayments were heavily penalized.
- Liquidated wallets dropped 20 points per liquidation.

# 🎯 Conclusion

This scoring model helps identify reliable vs risky DeFi users based on real on-chain behavior.
