# ⚾ MLB Game Winner Predictor using Machine Learning

This project uses machine learning to predict the winners of Major League Baseball (MLB) games based on historical performance, player statistics, and stadum. It's designed for sports enthusiasts, data scientists, and anyone interested in the application of machine learning for prediction.

## 📌 Features
- Predicts the outcome of MLB games (win/loss)

- Utilizes historical stats (e.g.,  xwoba, team batting average)

- Machine Learning models include: SVC, NearestCentroid, XGBoost, MLP, and Gradient Boosting.

- Model evaluation using accuracy

## 🧠 Machine Learning Approach

### 📊 Data Sources

- [MLB Savant](https://baseballsavant.mlb.com/gamefeed) – Advanced Statcast data (player-level)
- [Retrosheet](https://www.retrosheet.org/gamelogs/index.html#) – Historical game outcomes

### 📌 Features Used

**Batting Metrics**:
- `xwOBA`
- `K%` (strikeout rate)
- `BB%` (walk rate)
- `HardHit%`
- `Barrels/PA%`
- `Launch Speed`
- `Bat Speed`

**Pitching Metrics**:
- `xwOBA`
- `K%`, `BB%`
- `Barrels/BBE%`
- `Velocity`
- `Spin Rate`
- `Swing & Miss%`

**Contextual Features**:
- Stadium (home field)
- Game time (day/night)

---

## 🗂️ Project Structure

```
MLB-Game-Winner-Predictor/
├── 2024_Playoff_Cleaner/       # Cleans all 2024 Playoff matches, including Jupyter notebooks, raw and processed playoff data
├── 2025_Games_Cleaner/         # Only includes 2025 data for LAN and SDN includes Jupyter notebooks, raw data, processed data, and data templates
├── MLB_Reg_2024_Cleaner/       # Cleans all 2024 regular season games Jupyter notebooks, raw and processed playoff data
├── Savant_Cleaner/             # Cleans data from MLB Savant, includes Jupyter notebooks, raw and processed data from MLB Savant
├── Train_Test/                 # Jupyter notebooks for model training and predictions
├── ABV.csv                     # CSV file containing team abbreviations
├── ballpark/                   # Directory with ballpark code references
└── README.md                   # Project documentation and overview
```

## 📈 Model Performance

| Model                | Average Accuracy |
| -------------------- | ---------------- |
| Gradient Boosting    | **0.6045**       |
| Nearest Centroid     | 0.5997           |
| XGBoost              | 0.5869           |
| SVC (Support Vector) | 0.5086           |
| MLP (Neural Net)     | 0.5086           |

Best model so far: Gradient Boosting

## Future Work

- Fine-tune existing models – Optimize hyperparameters to improve predictive accuracy and generalization.

- Experiment with additional models – Explore deep learning approaches (e.g., LSTMs or CNNs) and ensemble stacking.

- Use more current, context-specific data – Instead of full-season stats, use stats prior to each game for more realistic, real-time predictions.

- Integrate betting odds – Incorporate sportsbook data to compare model predictions with public expectations and identify value betting opportunities.

## Contact 
- Feel free to reach out for questions or comments.

