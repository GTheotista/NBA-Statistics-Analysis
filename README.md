# NBA Statistics Analysis

## **Project Overview**
This project analyzes NBA player performance statistics during the 2023-2024 regular season. The dataset contains over 400 players and 30 statistical metrics, focusing on identifying key trends in player performance across different timeframes. The goal is to provide insights into player consistency, team performance, and statistical trends over the season.

## **Dataset**
The dataset consists of multiple CSV files, each representing player statistics at different points in the season. For consistency and relevance, only data from the end of each month has been used.

## **Tools Used**
- **Programming Language:** Python
- **Libraries:** Pandas, NumPy, Scikit-learn, Statsmodels
- **Visualization:** Matplotlib, Seaborn

## **Project Workflow**
### **1. Data Understanding**
We analyze key statistical features, including:
- **PTS** (Points per game)
- **AST** (Assists per game)
- **TRB** (Total rebounds per game)
- **FG%** (Field goal percentage)
- **3P%** (Three-point field goal percentage)

### **2. Data Preprocessing**
- **Handling Missing Values:**
  - Missing values in shooting percentages are recalculated from base metrics.
  - Players appearing in multiple teams are aggregated under `Tm=TOT`.
- **Feature Engineering:**
  - New columns are created for tracking player transfers.
  
### **3. Statistical & Trend Analysis**
- **Linear Regression**
  - Identifies player performance trends based on total points, assists, and rebounds.
- **ANOVA Testing**
  - Tests for significant performance variations across months.

### **4. Key Findings**
- **Brooklyn Nets, Indiana Pacers, and Phoenix Suns** show the most consistent scoring trends, while **New York Knicks** has the lowest average points.
- **Indiana Pacers lead in assists**, followed by **Miami Heat and Cleveland Cavaliers**, with **New York Knicks** ranking the lowest.
- **Boston Celtics, Brooklyn Nets, and Charlotte Hornets** dominate in rebounds, while **Washington Wizards** rank the lowest.

### **5. ANOVA Test Results**
- **Total Points:** F=1300.87, p-value=1.53e-65 (Significant variation)
- **Total Assists:** F=640.44, p-value=8.93e-53 (Significant variation)
- **Total Rebounds:** F=1351.11, p-value=3.09e-66 (Significant variation)

These results confirm that performance metrics vary significantly across months, indicating dynamic shifts in player and team effectiveness.

## **Conclusion**
- Team and player performance fluctuates significantly over time.
- Certain teams and players maintain consistency, while others show drastic changes.
- Future improvements could include more in-depth feature engineering, predictive modeling, and tracking player efficiency ratings.

---
**Author:** [Your Name]

