<<<<<<< HEAD
# 🏠 California Housing Prices — Random Forest Regressor

A machine learning project that predicts median house values (in $100,000s) using the California Housing dataset from Scikit-learn.

---

## Dataset

Source: [California Housing Dataset — Scikit-learn](https://scikit-learn.org/stable/datasets/real_world.html#california-housing-dataset)

| Feature | Description |
|---|---|
| `MedInc` | Median income in block group |
| `HouseAge` | Median house age |
| `AveRooms` | Average number of rooms |
| `AveBedrms` | Average number of bedrooms |
| `Population` | Block group population |
| `AveOccup` | Average house occupancy |
| `Latitude` | Block group latitude |
| `Longitude` | Block group longitude |
| `MedHouseVal` | **Target** — Median house value |

---

## Methodology

- **Split:** 80% training / 20% test
- **Algorithm:** `RandomForestRegressor` (ensemble learning)
- **Key hyperparameters:** `n_estimators=100`, `random_state=42`

---

## Results

### Random Forest Regressor

| Set | MSE | MAE | R² | RMSE |
|---|---|---|---|---|
| Training | 0.0353 | 0.1221 | **0.9736** | 0.1879 |
| Test | 0.2556 | 0.3277 | **0.8050** | 0.5055 |

### Linear Regression (baseline comparison)

| Set | MSE | MAE | R² | RMSE |
|---|---|---|---|---|
| Training | 0.5179 | 0.5286 | 0.6126 | 0.7197 |
| Test | 0.5559 | 0.5332 | 0.5758 | 0.7456 |

---

## Conclusions

- **Random Forest > Linear Regression** — better R², lower errors on all sets.
- The model shows mild **overfitting** (R² drops from 0.97 on train to 0.80 on test), meaning it learned training patterns well but generalises with some loss.
- Varying `n_estimators` (50, 100, 200) yields no significant improvement — the dataset appears to be at performance ceiling with this approach.
- Low MSE, MAE, and RMSE values confirm **good overall model performance**.

---

## Tech Stack

`Python` · `Scikit-learn` · `Pandas` · `Matplotlib` · `Jupyter Notebook`
=======
# California-housing-price-prediction
tema1 TIA
>>>>>>> cccc1c5045bbd4bffb5f382cb01b6b3330975365
