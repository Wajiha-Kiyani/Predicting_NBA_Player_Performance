
# Data Preprocessing, Model Building and Prediction Analysis

## Project Overview:
This project analyzes the **NBA Players Performance Dataset** to predict NBA player performance using various regression models. The dataset includes player statistics like points, assists, rebounds, and shooting efficiency. The project demonstrates data preprocessing, feature engineering, model building and evaluation.

## Dataset:
- **Dataset Name:** NBA Players Performance Dataset
- **Key Features:**
  - **Player Information:** Name, Position, Age, Team.
  - **Game and Performance Metrics:** Games played, Field goals, Three-point shooting, Rebounds, Assists, Steals, Blocks, Turnovers, Points scored.
  - **Key Performance Metrics:** Points (PTS), Assists (AST), Rebounds (TRB), Field Goals (FG%), 3-point shooting (3P%), Free Throws (FT%).

## Steps Involved:
1. **Loading Important Libraries:** 
   - Required libraries include `pandas`, `numpy`, `matplotlib`, `seaborn`, and `scikit-learn`.

2. **Loading Dataset:**
   - Dataset is loaded using `pd.read_csv()`.

3. **Exploring the Dataset:**
   - Displays the first and last five rows, dataset shape, column names, data types, and missing values.

4. **Generating Summary Statistics:**
   - Extracts statistical summaries like mean, standard deviation, and percentiles for key columns.

5. **Exploratory Data Analysis (EDA):**
   - Visualizes the distribution of key stats and correlation heatmap of important metrics.

6. **Feature Engineering:**
   - New features like `Recent_Performance` and `Scoring_Efficiency` are generated.
   - Missing values are imputed with column medians.
   - Features are standardized using `StandardScaler`.

7. **Feature Selection:**
   - Correlation analysis is done, and the most influential features are identified using Random Forest.

8. **Model Training and Evaluation:**
   - **Linear Regression** and **Ridge Regression** are trained and evaluated based on **R-squared** and **Mean Absolute Error (MAE)**.

9. **Feature Analysis:**
   - Key features like **FGA**, **FG%**, **TRB**, and **AST** are analyzed as predictors of player performance.

## Requirements:
- Python 3.x
- Libraries: `pandas`, `numpy`, `matplotlib`, `seaborn`, `scikit-learn`

You can install the required libraries using the following command:
```bash
pip install pandas numpy matplotlib seaborn scikit-learn
```

## How to Run the Code:
1. Download the **NBA Players Performance Dataset** CSV file and place it in the same directory as the script.
2. Clone or download the repository containing the code.
3. Open the notebook or script and run each cell step by step.
4. The dataset will be loaded, processed and used for regression modeling.
5. The results, including model evaluation metrics and feature importance, will be printed and visualized.

## Conclusion:
This project demonstrates how data preprocessing, feature selection and regression analysis can be applied to predict NBA player performance. By evaluating key features like shooting efficiency and rebounds, the model successfully predicts a player's points scored based on various performance metrics.
