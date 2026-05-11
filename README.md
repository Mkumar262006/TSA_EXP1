# Ex.No: 01A PLOT A TIME SERIES DATA
### REG NO : 212223240082
###  Date: 11-05-2026

# AIM:
To Develop a python program to Plot a time series data (population/ market price of a commodity
/temperature.
# ALGORITHM:
1. Import the required packages like pandas and matplot
2. Read the dataset using the pandas
3. Calculate the mean for the respective column.
4. Plot the data according to need and can be altered monthly, or yearly.
5. Display the graph.
# PROGRAM:
```py
import pandas as pd
import matplotlib.pyplot as plt

# Load the dataset
df = pd.read_csv("/content/matches.csv")

# Create yearly match count using season column
yearly_data = df.groupby('season')['id'].count()

# Plot the graph
yearly_data.plot(kind='line', marker='o')

plt.title('IPL Matches Played Per Season')
plt.xlabel('Season')
plt.ylabel('Number of Matches')
plt.grid(True)

plt.show()
```
# OUTPUT:
<img width="832" height="588" alt="image" src="https://github.com/user-attachments/assets/3d9d7ad7-7a33-4c17-9ca5-8c2744c7d5a7" />
# RESULT:
Thus we have created the python code for plotting the time series of given data.
