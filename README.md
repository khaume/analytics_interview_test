# Coding exercise
The following exercise will try to quickly assess your modelling and data science skills, how you deal with timeseries data, illustrate how some of our activities take place, and be base for discussion during the interview.

## Introduction
An important activity for Ørsted is to buy and sell power on the European markets, therefore having an informed view on the future production of power allows for a competitive advantage when placing bids and offers. One of the inputs to this view comes from production forecast for Ørsted’s windfarms provided by a number of vendors. These vendors take into account the location of the windfarms, the placement of the wind turbines, the weather, and other factors and then provide daily forecast for the production for the windfarms for the next 24-hour period.

This task is about trying to predict the true production based on three forecasts.

## Data
This repository contains two pickle files, `features.pkl` and `target.pkl`. 

`features.pkl` is a time-indexed Pandas dataframe with three columns, 0, 1, and 2. The values represent the forecasted production from three forecast vendors for a portfolio of Ørsted windfarms (data has been transformed from its original). The units are MWh for the 30-minute window given by the index.
`target.pkl` contains the actual production from the portfolio for the same time range.

##  Task
Your task is to create a Python class with an `sklearn`-style API (at least `fit`, `predict`, and `score` methods should be implemented) to predict the actual production based on the forecasted productions from the three vendors.

There is no limitation in terms of modelling techniques, feature engineering/cleaning, or extra data you may want to include. If you do include extra data, please add this to the submission.
Likewise, please add a `requirements.txt` file for any packages that are needed to run your code.

If the model takes more than 10 minutes to train on a normal laptop, then please add a method in the class to load a pre-trained model (e.g. by pickling it).

We will evaluate:
-	Feature engineering and model creation
-	Code quality
-	Score of the model

Additionally, it is a plus if you add unit tests of your code.

## Delivery
Please reply to the email, from which you got the link to this repo, with a link to a GitHub or GitLab repo containing your code, cc: kahau@orsted.dk.
