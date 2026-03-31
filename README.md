# Euromillones Participation Analysis
Analyzing historical participation patterns in the Euromillones lottery and predicting trends using regression models.

## Motivation
The goal is to understand how participation varies over time and according to different factors such as jackpot size, day of the week, and seasonal trends. 
This allows us to explore cyclic patterns and predict participation behavior. This pattern is important since in Spain there is an extra price ('EL MILLON') of 1 million euros always randomly selected from the tickets that are sold. Hence, the lower the participation, the higher the probability to get this price. 

## Data
- Source: Euromillones historical data (https://www.loteriasyapuestas.es/es/resultados/euromillones)
- Preprocessing:
  - Data cleaning with Pandas
  - Feature engineering: day of the week, day of the year as cyclical variables, jackpot size
  - Outlier detection using scatter and boxplots
- Tools: Python, Pandas, Matplotlib, Seaborn

## Methods
- Models applied:
  - Linear Regression
  - Random Forest Regressor
- Model evaluation:
  - Cross-validation using `cross_val_score`
  - RMSE comparison
- Visualization of participation patterns across the year and by day of the week

## Results
- Participation shows clear weekly and seasonal patterns
- Tuesdays with medium jackpot tend to have lower participation (around 20 April observed)
- Regression models capture main trends but randomness of lottery remains high

## How to Run
1. Clone the repository
2. Install dependencies: `pandas`, `numpy`, `scikit-learn`, `matplotlib`, `seaborn`
3. Run the notebook:
```bash
jupyter notebook Euromillones_analisis.ipynb
