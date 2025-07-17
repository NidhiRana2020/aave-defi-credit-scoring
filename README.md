# Aave DeFi Wallet Credit Scoring

## 📊 Problem Statement

Build a robust ML model to assign a **credit score (0-1000)** to wallets using their transaction behavior on Aave V2.

## 🏗️ Methodology

1. **Data Ingestion:** Loaded 100k+ transactions from provided JSON.
2. **Feature Engineering:**
   - Sum of deposits, borrows, repayments
   - Number of transactions
   - Number of liquidations
   - Tenure (days active)
3. **Credit Scoring Logic:**
   - Rewards high deposits, repayments, longer tenure
   - Penalizes liquidations, high borrow without repay
4. **Scoring:** Scaled between 0-1000 using engineered rules.
5. **Output:** `wallet_credit_scores.csv` containing wallet addresses and scores.

## 📝 Files

- `aave_credit_scoring.ipynb` – Full Colab notebook
- `wallet_credit_scores.csv` – Final output
- `analysis.md` – Score distribution insights

## 🔧 Usage

```bash
# Clone repo
git clone https://github.com/NidhiRana2020/aave-defi-credit-scoring.git

# Open notebook in Colab or VS Code to re-run
