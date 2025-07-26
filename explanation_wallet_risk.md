# 📊 Explanation of Risk Scoring Model

## 1. Data Collection
- **Source:** Covalent API (Ethereum Mainnet)
- **Wallets:** 100 addresses from provided Google Sheet
- **Data fetched:** Transactions using `/transactions_v2` endpoint

## 2. Feature Engineering
Created a clean DataFrame with:
- `wallet`, `block_signed_at`, `from_address`, `to_address`, `value`, `gas_spent`, `gas_price`, `successful`

From this, engineered features:
- **num_txns**: Total number of transactions
- **num_successful_txns**
- **total_eth_sent**: Converted from Wei
- **avg_gas_price**
- **num_inbound / outbound txns**
- **days_since_last_tx**

## 3. Normalization
- Used `MinMaxScaler` to scale features between 0–1
- Re-weighted based on risk relevance

## 4. Scoring
- Score = weighted sum of normalized features
- Inverted for risk direction (e.g., more outbound = riskier)
- Final score scaled from 0–1000

## 5. Output
- Final CSV has:
  - `wallet_id`
  - `score` (0–1000)

