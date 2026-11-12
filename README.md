# San Diego Padres Demo

A sample project built for the San Diego Autism Tree Project. It analyzes San Diego Padres franchise batting data from 1969 to 2023 ([Kaggle dataset](https://www.kaggle.com/datasets/mattop/san-diego-padres-batting-and-pitching-1969-2023)).

## Repository Contents

| File | Description |
|---|---|
| `Demo for San Diego Autism Tree Project (San Diego Padres Batting).ipynb` | Full demo: cleaning, visualization, franchise leaders and a classification model |

## Commit History

### `20b6f68`: Upload of the Padres demo notebook (2025-12-14)
- **Cleaning:**
  - dropped the rank column and checked for nulls and duplicates
  - removed pitchers so the analysis covers position players only
  - added infielder and outfielder columns
  - renamed the 2009–2010 Tony Gwynn records to Tony Gwynn Jr.
- **Visualizations:**
  - age histogram: the most common age range is 22.5–25
  - batting average by position: corner and center outfielders and third basemen hit higher than catchers and DHs
  - home runs and runs scored per season (line graphs)
- **Franchise leaders and players:**
  - top 10 in hits and home runs, noting that Manny Machado has since become the franchise home run leader
  - average production by position group
  - comparisons of Fernando Tatis Jr., Manny Machado and Jake Cronenworth
  - Eric Hosmer's production across seasons
  - Tony Gwynn's batting average vs. hits and at-bats
- **Classification: predicting whether a hitter bats left-handed from batting stats, with logistic regression:**

  | Model | Accuracy |
  |---|---|
  | Logistic regression (base) | 72.0% |
  | `LogisticRegressionCV` (10-fold) | 74.2% |
  | Best k-fold cross-validation score | 81.7% |

## Tools
Python, pandas, NumPy, scikit-learn, matplotlib, seaborn, Jupyter Notebook
