## import matplotlib and pandas

from matplotlib import pyplot as plt

import pandas as pd

## load dataset

line_data = pd.read_csv('data.csv')

line_data.head()

## line graph 

plt.plot(line_data.month_name,line_data.windhoek_avg_high)

## show the plot

plt.show()


## Display Issues
The plt.show() call is correct, but if you're running this in a non-interactive environment (e.g., a script), ensure it's included to display the plot.

In some environments (e.g., Jupyter notebooks), you might need %matplotlib inline to render plots.

Fix: If in a Jupyter notebook, add:

%matplotlib inline

