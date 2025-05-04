# import matplotlib and pandas

from matplotlib import pyplot as plt

import pandas as pd

# load dataset

line_data = pd.read_csv('data.csv')

line_data.head()

## line graph ##

plt.plot(line_data.month_name,line_data.windhoek_avg_high)

## show the plot

plt.show()
