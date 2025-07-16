{
 "cells": [
  {
   "cell_type": "markdown",
   "id": "ac2f84d9-2d0a-4670-8488-f717c15e8c3a",
   "metadata": {},
   "source": [
    "# Aave V2 Wallet Credit Scoring\r\n",
    "\r\n",
    "This project assigns a credit score (0–1000) to each wallet based on its transaction behavior on the Aave V2 protocol using DeFi transaction data.\r\n",
    "\r\n",
    "## 🚀 Overview\r\n",
    "\r\n",
    "Each wallet interacts through actions such as:\r\n",
    "- `deposit`\r\n",
    "- `borrow`\r\n",
    "- `repay`\r\n",
    "- `redeemunderlying`\r\n",
    "- `liquidationcall`\r\n",
    "\r\n",
    "We analyze these patterns and score them for creditworthiness.\r\n",
    "\r\n",
    "## 🔍 Steps Followed\r\n",
    "\r\n",
    "1. Loaded and parsed JSON transaction data.\r\n",
    "2. Engineered features: deposit/borrow/repay counts, totals, active days.\r\n",
    "3. Applied a custom scoring function based on user activity.\r\n",
    "4. Generated `wallet_scores.json`.\r\n",
    "5. Plotted wallet score distribution as `score_distribution.png`.\r\n",
    "\r\n",
    "## 📦 Output Files\r\n",
    "\r\n",
    "- `wallet_scores.json` – Scores for each wallet\r\n",
    "- `score_distribution.png` – Histogram of credit scores\r\n",
    "\r\n",
    "## 💡 How to Run\r\n",
    "\r\n",
    "Open `score_runner.ipynb` or `score_runner.py` and run all cells.\r\n",
    "\r\n",
    "## 📬 Author\r\n",
    "\r\n",
    "Kamalalaya Gummadi\r\n"
   ]
  }
 ],
 "metadata": {
  "kernelspec": {
   "display_name": "Python [conda env:base] *",
   "language": "python",
   "name": "conda-base-py"
  },
  "language_info": {
   "codemirror_mode": {
    "name": "ipython",
    "version": 3
   },
   "file_extension": ".py",
   "mimetype": "text/x-python",
   "name": "python",
   "nbconvert_exporter": "python",
   "pygments_lexer": "ipython3",
   "version": "3.12.4"
  }
 },
 "nbformat": 4,
 "nbformat_minor": 5
}
