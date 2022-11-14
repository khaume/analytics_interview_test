# Coding exercise
The purpose of the following exercise is to assess your data analytical skills, how you 
deal with timeseries data and illustrate findings, and also to illustrate how some of our 
activities take place, and lastly to be basis for discussion during the interview.

## Introduction
An important activity for Ørsted is to buy and sell power on the European markets. Having an
informed view on the future production of power therefore allows for a competitive advantage when
placing bids and offers. 
One of the inputs to this view comes from production forecast for Ørsted's 
windfarms provided by a number of vendors. These vendors take into account the location of the 
windfarms, the placement of the wind turbines, the weather, and other factors and then provide 
daily forecast for the production for the windfarms for the next 24-hour period.

## Data
This repository contains two pickle files, `features.pkl` and `target.pkl`. 

`features.pkl` is a time-indexed Pandas dataframe with three columns, `0`, `1`, and `2`. The values 
represent the forecasted production from three forecast vendors for a portfolio of Ørsted windfarms 
(data has been transformed from its original). The units are MWh for the 30-minute window given by 
the index.
`target.pkl` contains the actual production from the portfolio for the same time range.

##  Task
Your task is to analyze the data and present your conclusions from the data in a way you feel conveys 
the message in the strongest way.

There is no limitation in terms of techniques, feature engineering/cleaning, or extra data 
you may want to include. If you do include extra data, please add this to the submission.
Likewise, please add a `requirements.txt` file for any packages that are needed to run your code.

We will evaluate:
- Code quality and any unit tests of your code you may wish to add.
- Your ability to convey a meaningful and clear message from the data

You will be asked to talk about and go through your solution which you can do just by going through
your source code or in the form of a Jupyter notebook if that helps you present (we will look at
source code either way).


### Additional questions

Please also be ready to talk about/discuss the following

**Domain**
- What is the average weekly production? Does this number sound fair?
- Would you expect seasonality in this kind of data? If so, why and what kind?
- If you had been able to ask questions about the domain, would that have helped you? What
 questions would you have asked?
- If we assume Ørsted buys actulas at spot price (N2EX) and sell at a mix of spot (N2EX) and 
imbalance price (SIP), how would you conduct an analysis for sizing the balancing fee (management
fee) to make the profit go to zero.

**Technical**
- Argue why you chose the presentation form you did?
- If you had had more time, what would you have done?


## Delivery
Please reply to the email, from which you got the link to this repo, with a link to a GitHub or
 GitLab repo containing your code, and please cc: `kahau@orsted.com`.
