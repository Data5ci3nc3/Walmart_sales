## Walmart sales project
Build a machine learning model able to predict the weekly sales in Walmart stores with the best possible precision.

## Goals to be achieved
- Conduct exploratory data analysis (EDA) and make all necessary preprocessings to prepare data for machine learning
- Train a linear regression model (baseline)
- Avoid overfitting by training a regularized regression model

## Methodology applied to reach the goal
- Creating a baseline model
- Plotting feature importance
- Creating a ridge-regularized model without hyper parameter optimization
- Ridge-regularized model with hyper parameter optimization
- Summary of the three models (R2 score on training set and R2 score on test set)

## Conclusion
- In Machine learning, depending on the problem to be solved, basic models can sometimes outperform more complex ones.

- Training a model with a small amount of data will produce misleading scores. It is not beacause our model gives a R2 score of 98 % at the first try that we should think that the model is the best model ever. We should investigate and try to understand what is going on under the hood. The three models designed for the purpose of this project perform more or less correctly despite the fact that they have been trained with limited data. Nevertheless, training these models with more data would have helped them generalize better - prevent overfitting - and make better predictions.

- Machine learning being an iterative process and no model being a priori guaranteed to work better, we can experiment with different models to see if they produce better scores. It is better to run the model and record its scores rather than making assumptions about a particular model's performance.
