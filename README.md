# Used Car Price Prediction with Linear Regression

Adding the car’s model name reduced mean absolute error from **$5,564 to $4,296** on the test set, a **23% reduction** compared with the log price model that omitted the model name.

[Open the Jupyter notebook](used_car_price_prediction%20%281%29.ipynb)

## What I tested

I used Python and linear regression to estimate used car prices. I wanted to see whether the car’s specific model added useful information beyond its brand and whether training on log prices improved predictions.

I used the same 3,093 training rows and 774 test rows for all three comparisons:

- Log prices without the car’s model name
- Log prices with the car’s model name
- Raw dollar prices with the car’s model name

## What I found

The model trained on log prices with the car’s model name had the lowest error on this test split. For the 24 test cars whose model names were absent from the training data, however, adding that feature increased average error. Training directly on raw prices also increased overall error and produced 54 negative price estimates.
