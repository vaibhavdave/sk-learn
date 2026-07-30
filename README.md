# sk-learn

A structured, hands-on syllabus for learning classic machine learning algorithms:
**theory first, then implementation and evaluation with scikit-learn**, inside
Jupyter notebooks with visualizations to build intuition.

## How each notebook is organized

1. **Theory** — intuition, core math/formula, assumptions, pros/cons, when to use it
2. **Implementation** — the algorithm applied to a real or synthetic dataset via sklearn
3. **Evaluation** — relevant metrics and diagnostic plots
4. **Exercises** — small variations to reinforce the concept

## Setup

```bash
python3 -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt
jupyter notebook
```

## Syllabus

| Module | Topic |
|---|---|
| [00_foundations](00_foundations) | ML types, bias-variance tradeoff, overfitting/underfitting, train/test split & cross-validation concepts |
| [01_data_preprocessing](01_data_preprocessing) | Missing values, encoding, scaling, CV strategies, regression & classification evaluation metrics |
| [02_regression](02_regression) | Linear, Ridge/Lasso/ElasticNet, Polynomial, Decision Tree, Random Forest, Gradient Boosting, SVR |
| [03_classification](03_classification) | Logistic Regression, KNN, Naive Bayes, Decision Trees, SVM, Random Forest |
| [04_ensemble_methods](04_ensemble_methods) | Bagging, AdaBoost, Gradient Boosting, Voting, Stacking |
| [05_unsupervised_learning](05_unsupervised_learning) | K-Means, Hierarchical Clustering, DBSCAN, PCA, t-SNE, Anomaly Detection |
| [06_model_selection_tuning](06_model_selection_tuning) | Pipelines, GridSearchCV/RandomizedSearchCV, learning & validation curves |
| [07_imbalanced_and_feature_selection](07_imbalanced_and_feature_selection) | Class weights, SMOTE, feature importance, RFE, SelectKBest |
| [08_neural_nets_intro](08_neural_nets_intro) | sklearn's MLPClassifier/MLPRegressor (bridge topic, not full deep learning) |
| [09_capstone_project](09_capstone_project) | End-to-end project applying the full pipeline to a real dataset |

Datasets used are small, well-known sklearn built-ins (iris, wine, breast cancer,
california housing, diabetes) or synthetic (`make_classification`, `make_regression`,
`make_blobs`) so every notebook runs quickly with no external downloads.
