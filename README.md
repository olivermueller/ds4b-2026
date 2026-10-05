# Data Science for Business (ds4b-2026)

Paderborn University · Winter Term 2026/27 · (c) Oliver Mueller

Jupyter notebooks for the in-class sessions. The course follows
*An Introduction to Statistical Learning with Applications in Python* (ISLP) by James, Witten, Hastie, Tibshirani and Taylor (Springer, 2023), freely available at [statlearning.com](https://www.statlearning.com).
Before each session, watch the corresponding videos of the ISLP online course. In class, we go through the notebooks together.

## Sessions

| Session | Notebook(s) | Topic | ISLP |
|---|---|---|---|
| 1 | `credit_card_default_knn` | K-nearest neighbors, train/test split, confusion matrix | Ch. 2 (2.2.3), 4.4.2, Lab 4.7.6 |
| 2 | `nycflights_prep_and_viz` | Data preparation, joins, visualization | Lab 2.3 (joins go beyond ISLP) |
| 3 | `ames_linear_regression`, `gradient_descent` | Linear regression, gradient descent | Ch. 3, 10.7, Lab 3.6 |
| 4 | `micromortgage_logit` | Logistic regression, ROC/AUC, cross-validation | Ch. 4 (4.3, 4.4.2), 5.1, Labs 4.7, 5.3 |
| 5 | `ames_subset_selection`, `ames_lasso` | Subset selection, lasso | Ch. 6 (6.1, 6.2, 6.4), Lab 6.5 |
| 6 | `ames_gam` | Generalized additive models | Ch. 7 (7.5, 7.7), Lab 7.8.3 |
| 7 | `micromortgage_tree-based_models`, `micromortgage_stacking_w_meta` | Trees, random forests, boosting, stacking | Ch. 8, Labs 8.3 (stacking goes beyond ISLP) |
| 8 | `ames_mlp_scikit`, `ames_mlp_pytorch` | Neural networks (MLP) | Ch. 10 (10.1, 10.2, 10.7), Lab 10.9.1 |
| 9 | `fashionmnist_mlp_pytorch`, `fashionmnist_cnn_pytorch` | Image classification, CNNs | Ch. 10 (10.3), Labs 10.9.2–10.9.3 |
| 10 | `wine_mlp_tensorflow`, `wine_rnn_tensorflow` | Text data, embeddings, RNNs/LSTMs | Ch. 10 (10.4, 10.5), Labs 10.9.5–10.9.6 |
| 11 | – | (no notebook) | |
| 12 | `ames_interpretable_ml` | Interpretable ML: permutation importance, PDP/ICE, SHAP | 2.1.3, 8.2.1 · beyond ISLP: Molnar, *Interpretable Machine Learning* |
| 13 | `germancredit_fair_ml` | Fair ML: fairness metrics, bias mitigation | beyond ISLP: Barocas, Hardt & Narayanan, *Fairness and Machine Learning* |

## Running the notebooks

**Google Colab (recommended):** open a notebook from this repository via *File → Open notebook → GitHub*. All data is loaded from this repository's raw URLs. Packages that Colab doesn't ship are listed in a commented `# !pip install ...` line at the top of each notebook; uncomment and run it.

**Locally:** Python 3.11 or 3.12.

```bash
pip install -r requirements.txt
jupyter lab
```

## Data sources

- `default.csv`: ISLP `Default` data
- `flights.csv`, `airlines.csv`, `airports.csv`, `planes.csv`, `weather.csv`: R package `nycflights13`
- `ameshousing.csv`: Ames Housing data (De Cock, 2011)
- `advertising.csv`: ISLP `Advertising` data
- `micromortgage.csv`: micro-mortgage applications (see `variables.pdf`)
- Fashion-MNIST (Zalando Research): downloaded by `torchvision`
- `winemag-data-130k-v2.csv`: Wine Enthusiast reviews (Kaggle)
- German Credit: UCI Machine Learning Repository, via `aif360`
