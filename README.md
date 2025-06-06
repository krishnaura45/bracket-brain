# 🏀bracket-brain
Forecasting NCAA basketball tournament outcomes using machine learning models to support bracket predictions and sports analytics.

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Kaggle](https://img.shields.io/badge/Kaggle-20BEFF?style=for-the-badge&logo=kaggle&logoColor=white)
![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white)
![Brier Score Optimized](https://img.shields.io/badge/Optimized--for-Brier%20Score-yellowgreen?style=for-the-badge)
![Metric Score](https://img.shields.io/badge/Best%20Score-0.10921-2ECC71?style=for-the-badge)
![Rank](https://img.shields.io/badge/Rank-53%20of%201727-brightgreen?style=for-the-badge)
![Solo](https://img.shields.io/badge/Submission-Solo-orange?style=for-the-badge)

### **Project Duration**: Mar 17, 2025 - Apr 7, 2025

---

## 🧠 Problem Statement

The aim of this competition was to predict the outcomes of all potential matchups in the 2025 NCAA Division I men’s and women’s basketball tournaments. Each submission included predicted probabilities for every possible matchup that could occur in the tournament brackets. 

Hosted on Kaggle as part of the annual **March Machine Learning Mania**, submissions were evaluated using the **Brier score**, which penalizes inaccurate probability predictions. Lower Brier scores indicate better predictions.

---

## 🧩 Approach

You can explore the complete methodology in this notebook: 🔗 [MMLM25 - EDA and Prediction](https://github.com/krishnaura45/bracket-brain/blob/main/mmlm25-eda-pred.ipynb)

Key steps followed:

- 📊 **Exploratory Data Analysis (EDA)**:
  - Understood tournament structure, team seeding, and regional splits.
  - Analyzed match histories and evaluated metrics such as `ScoreDiff`, `SeedDiff`, and team-level historical performance.
  - Assessed other features such as win-loss records, and scoring statistics.

- 🧠 **GOTO Model**:
  - Utilized the goto_conversion method to convert betting odds into outcome probabilities.
  - This method adjusts inverse odds by the same units of standard error, effectively addressing the favourite-longshot bias by considering the proportionately wider standard errors implied for inverses of longshot odds and vice versa.

- 🧪 **Prediction & Submission**:
  - Mapped test data using team identifiers from the sample submission file.
  - Applied the converted probabilities to predict outcomes for every possible tournament matchup.
  - Ensured that the predictions accounted for the inherent biases in betting markets, leading to more accurate forecasts.

---

## 🏆 Results / Outcomes

- ✅ **Public Leaderboard Scores**:
  - Achieved **0.12453** and **0.10921** Brier scores.

- 🏁 **Private Leaderboard Score**:
  - Final score: **0.10921** on hidden test data.

- 🥇 **Rank Achieved**:
  - Placed **53rd out of 1,986 participants** and **1,727 teams** as a **solo participant**.

---

## 🔗 References

- 🏆 Kaggle Competition: [March Machine Learning Mania 2025](https://www.kaggle.com/competitions/march-machine-learning-mania-2025)
- 📁 Dataset: [Competition Data](https://www.kaggle.com/competitions/march-machine-learning-mania-2025/data)
- 🗒️ Helpful Notebooks:
  - [MMLM - Starter by Paul](https://www.kaggle.com/code/paultimothymooney/simple-starter-notebook-for-march-mania-2025)
  - [Vilnius NCAA by Raddar](https://www.kaggle.com/code/jocelyndumlao/march-ml-mania-2025-brier-score-prediction)
- 📦 `goto_conversion` Package: [GitHub repo](https://github.com/gotoConversion/goto_conversion)

---

## 🛠️ Tech Stack

- **Language**: Python 🐍
- **Libraries**:
  - `pandas`, `numpy` for data manipulation
  - `matplotlib`, `seaborn` for visualization
- **Tools**:
  - Jupyter Notebook 📓 for development
  - Kaggle Kernels / Google Colab for experimentation and submission

---

📌 *This project highlights the effectiveness of advanced odds conversion techniques, like goto_conversion, in improving the accuracy of probabilistic forecasts for sports tournaments.*
