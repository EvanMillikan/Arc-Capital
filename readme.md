# Arc Capital Recruitment Task

Script & Visualization -> notebook/01_arc_capital.ipynb

# Thought Process

Coming in to this exercise, I determine the goal of the project. Which is to determine whether variable Skew is correlation with variable 30 day price change. So, in the beginning I decided that a model is not needed. A model can be built if the correlation is high just to see whether the Skew is useful enough to predict 30 day price change. Since the data is small, a neural net based model such as RNN or LSTM is not suitable so if a model is going to built most probably its going to be a statistical model.

I perform stationarity testing and stationarize the price value because in a time-series setting prediction cannot be done on non-stationary data. The easiest method to see whether two variables are cross-correlated in time-series setting is to look at their scatter plot. However, the scatter plot does not seem to show a trend. This is also further proven by checking their pearson correlation value.

Due to the two variable not being highly correlated, it is not useful to move to the next stage which is model training.

# Analysis

The Skew data does not show a decent usefulness in predicting bitcion 30 day price change. Using pearson correlation, it is only 7% inverse correlated, and looking directly using scatter plot there are no obvious trend between the two. If combined with other features, Skew can actually be useful as a feature in a machine learning model to predict the price change. However, alone it is too weak to be used to predict the price change.