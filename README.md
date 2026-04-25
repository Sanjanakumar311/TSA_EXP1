# Ex.No: 01A PLOT A TIME SERIES DATA
###  Date: 25-04-2026

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
from matplotlib import pyplot as plt
import pandas as pd

# Load dataset
df = pd.read_csv("/content/Social_media_impact_on_life.csv")

# Check first rows
print(df.head())

# Use index as x-axis (since no date column)
df.reset_index(inplace=True)

# Plot Avg Daily Usage Hours
plt.figure()
plt.plot(df['index'], df['Avg_Daily_Usage_Hours'], label='Daily Usage (Hours)')

plt.title('Average Daily Social Media Usage')
plt.xlabel('Student Index')
plt.ylabel('Usage Hours')
plt.legend()
plt.grid(True)

plt.show()

# OUTPUT:


<img width="876" height="611" alt="4353519f-b9ae-4668-b972-876533e41373" src="https://github.com/user-attachments/assets/d66482ca-8558-4db8-8662-c8f09da787a8" />

<img width="851" height="460" alt="4e5e02bf-b512-4123-9f2b-d0d57c340ce9" src="https://github.com/user-attachments/assets/b609f65a-4cb8-497b-98d0-1ad16175f822" />

<img width="760" height="585" alt="22df177c-c389-4301-aa56-6906d0ece681" src="https://github.com/user-attachments/assets/03421b57-a7b4-44db-bc17-716e8089505e" />






# RESULT:
Thus we have created the python code for plotting the time series of given data.
