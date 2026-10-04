# ML_derivations

Each notebook writes a model as math, names every symbol, derives how it is fit, implements the
derivation in numpy with long variable names, and checks the result against scikit-learn.

| notebook | derives | checked against |
|---|---|---|
| 01_linear_regression | model, MSE, gradient, gradient descent, normal equation, R-squared | LinearRegression on housing |
| 02_logistic_regression | sigmoid, log-odds, log loss from likelihood, gradient, thresholds | LogisticRegression on breast_cancer |
| 03_regularization | ridge closed form and gradient, lasso by coordinate descent with soft thresholding, the diamond picture, elastic net | Ridge and Lasso on diabetes |
| 04_trees_and_boosting | SSE and Gini splits, a recursive tree class, boosting as gradient descent in function space, bagging vs boosting | DecisionTreeRegressor and GradientBoostingRegressor on housing |
| 05_production_pipeline_sql_python | SQL extract, peer z-scores, weighted ridge logistic from scratch, out-of-fold evaluation, scores written back to SQLite, a scoring function from a saved artifact | CMS-derived providers table |

Kernel: Python (medicare-fraud). Data: `../Homework/homework.sqlite`.
