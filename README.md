# unemp_anal_RFR
Unemployment analysis with Random Forest Regressor

_______________________________________________

## Informations:

### From the Project:

THe purpose of this project is to predict the unemployment rates of an USA county
from twitter data (word frequency, hourly user activity) with random forest regressor (RFR).

The code first half is preparing the data for RFR.
Second half is RFR training and prediction, finaly processing the results.

### This project contains:

- The full code, wich name is "unemp_anal_RFR_v02_171021.ipynb"
- Parameter search (for random forest) results and Ipython script for ploting in "param_plot_data_script" folder
- Plots in "plots" folder

### More

#### Data approach:

The idea behind predicting from word frequency data is that
if one regions people using certain words more often than people in other region,
we can classify regions with that words.

The same idea for hourly activity.
If in certain regions people send their messages earlier than people in other regions,
then lower unemployment rate likely, because people get up earlier to go their workplace.
This is just an example for the approach.

#### Searching parameters:

The main code contains a parameter search method to find the best parameters for RFR.
The plots are in the "plots/param_grid" folder.

### Teaser:

The results of the prediction:
![plot](../master/plots/wordsData01UnempPred.png)

Example for parameter search:
![param](../master/plots/param_grid/AvtivData01CorrMD.png)

The full RFR tree:
![tree](../master/plots/tree/tree.png)
