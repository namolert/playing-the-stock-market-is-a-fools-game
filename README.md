# playing-the-stock-market-is-a-fools-game

## Overview

The training data provided gives the daily percentage movement of stock prices for 422 companies from 05/04/2010 to 31/03/2022.

Your task it to predict the daily percent movement of the 422 companies on the 1st of April 2022. (The day after the last time point in the training data.)

Generative AI disclosure: ChatGPT was used to create the competition logo.

## Description

**You may use the RNN Lab 7 as starting notebook for this submission.**

You should create a model which is trained on the training data and that can predict the last April 1st 2022 values for the 422 companies given. A template submission file (with all 0.0 values) is provided that you should read, fill in your predicted values and then save.

**In addition you should use [Optuna](https://optuna.org/)** to do appropriate hyperparameter optimization to get as high a score (i.e. low MSE value) as possible for your predictions on hopefully a validation dataset (and the public Kaggle data).

**As a stretch goal, you should do some interpretation of your model using Captum** to try to understand what features the model is using.

Your notebook should be tidy, have good section headings and some Markdown description of what different sections are doing. It should also show any output that is generated (particularly if you do the Captum analysis) and have Markdown that says how you interpret the output.

In addition to submitting your predictions to this Kaggle competition (to get a score on the leaderboard), **you also need to submit your final Jupyter Notebook (including outputs) via the Moodle site.**

## Evaluation

The public leaderboard will score your predictions using MSE compared to the ground truth values for the first 221 companies. The private leaderboard will be released after the deadline and will score your predictions using MSE on the remaining 221 companies.

(You should be using your own validation dataset to optimise hyper-parameters and only use the public leaderboard data up to 5 submissions a day to test your predictions.)

## Submission File

For each ID in the test set, you must predict a probability for the TARGET variable. The file should contain a header and have the following format:

```
ID,        value
company_0, 0.0
company_1, 0.0
company_2, 0.0
etc.
```
