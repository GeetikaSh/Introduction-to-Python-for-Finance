# Introduction-to-Python-for-Finance

**boolean slice I:NUMERIC**\
*Find the mean*\
price_mean = np.mean(prices)
 
*Create boolean array*\
boolean_array = (prices > price_mean)\
print(boolean_array)

 
*Select prices that are greater than average*\
above_avg = prices[boolean_array]\
print(above_avg)

**boolean slice II: string**

*Create boolean array*\
boolean_array = (sectors == 'Health Care')\
print(boolean_array)

 
*Print only health care companies*\
health_care = names[boolean_array]\
print(health_care)

## Visualization

**Importing matplotlib and pyplot**

import matplotlib.pyplot as plt\
plt.plot(days,prices, color="red", linestyle="--")\
plt.show()

**Adding axis labels and titles**
import matplotlib.pyplot as plt\

plt.plot(days, prices, color="red", linestyle="--")\

plt.xlabel('Days')\
plt.ylabel('Prices, $')\

plt.title('Company Stock Prices Over Time')\

plt.show()

**Multiple lines on the same plot**

plt.plot(days, prices1, color='red')\
plt.plot(days, prices2, color='green')\

plt.xlabel('Days')\
plt.ylabel('Prices, $')\
plt.title('Stock Prices Over Time')\
plt.show()

**Scatterplots**

import matplotlib.pyplot as plt

plt.scatter(days, prices, color='green', s=0.1)

plt.show()





