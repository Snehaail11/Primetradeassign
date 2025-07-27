# Primetradeassign

# Sentiment vs Closed PnL Analysis

This project explores the relationship between **market sentiment classifications** and **trading performance**, measured by Closed PnL (Profit and Loss). Using real-world sentiment data, the analysis investigates whether emotional market states (like "Extreme Greed" or "Fear") have any measurable impact on profitability.

---

## Objective

To determine whether market sentiment correlates with Closed PnL and identify which emotional states (if any) tend to result in higher or lower profits.

---

## Dataset

- **Size**: 211,224 rows
- **Columns**: 
  - `date`: Trade or sentiment date  
  - `classification`: Market sentiment (e.g., Fear, Greed)  
  - `Closed PnL`: Profit/Loss for that trade  

---

## 🧼 Data Cleaning

- Removed 0 PnL rows (106,816 rows)
- Removed NaN values (0 rows)
- Final dataset size: **104,408 rows**

---

## Analysis Performed

1. **Group-wise aggregation**:
   - Calculated **average**, **median**, and **count** of Closed PnL for each sentiment class.
2. **Data Visualization**:
   - Bar plot of average Closed PnL per sentiment class.
3. **Sentiment Mapping**:
   - Converted sentiment to numeric scores:
     - `Extreme Fear` = 0, ..., `Extreme Greed` = 4
4. **Correlation Check**:
   - Computed Pearson correlation between sentiment score and Closed PnL.

---

## 📈 Key Insights

- Weak positive correlation (**r = 0.0064**) between sentiment and Closed PnL.
- Some emotional extremes (e.g., Extreme Greed) showed larger PnL fluctuations.
- No strong linear relationship; sentiment alone does **not predict profitability**.

---

## 📦 Libraries Used

- Python `pandas`
- `matplotlib`
- `seaborn`

---

## 📌 Conclusion

While market sentiment reflects the emotional state of the market, this analysis shows that it doesn’t strongly correlate with profitability. Traders should use sentiment in combination with other indicators for better decision-making.


---

