# NBA Playoff Performance Modeling

This project explores what makes NBA teams successful in the **playoffs** by analyzing advanced team statistics from **2000–2022**. Using both descriptive and predictive analysis—including **ridge regression** to handle collinearity—we identify which metrics best predict postseason wins.

---

## Project Objectives

- Understand which team metrics most correlate with playoff wins.
- Identify league-wide **trends over time** (e.g., pace, 3P rate).
- Use **ridge regression** to handle multicollinearity and estimate the importance of each feature.

---

## Key Findings

- **True Shooting % (TS%)**, **Net Rating (NRtg)**, and **Free Throw Rate** are top predictors of playoff success.
- **Pace** and **3PAr** have increased over time but are **not directly correlated** with wins due to era effects.
- Defensive discipline (low **DRtg**) and efficient scoring matter more than aggressive rebounding or fast pace.

---

## Data Cleaning

- Removed missing values and duplicate headers
- Excluded 2023 playoffs (incomplete data)
- Dropped irrelevant columns (`Rk`, `PL`, `PW`)

---

## Modeling Approach

- Standardized numeric features
- Used **Ridge Regression** to model playoff win percentage
- Calculated **feature importance** using model coefficients
- Evaluated model fit using **R² and MSE**

---

## Project Structure

- NBAProject_Final.ipynd: Jupyter Notebook
- WL_playoff_total.csv: Publicly available NBA Playoff Team Data from Kaggle
- nba_playoff_performance_modeling.pdf: Written Report

---

## How to Run

1. Clone the repo
git clone https://github.com/yourusername/nba-playoff-modeling.git
cd nba-playoff-modeling

2. Set up a virtual environment (optional)
python3 -m venv venv
source venv/bin/activate

3. Install dependencies
pip install -r requirements.txt

4. Run the notebook
jupyter notebook NBAProject_Final.ipynd

---

## Dependencies

pandas, numpy, matplotlib, seaborn, scikit-learn, statsmodels

---

## Author
Beckett Newton
<br/>
bmn4602@nyu.edu
<br/>
linkedin.com/in/beckett-newton/
<br/>
datascienceportfol.io/beckettnewton
