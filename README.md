# Ex.No: 01A PLOT A TIME SERIES DATA
###  Date: 14-02-2026

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

### Name : Prakash C
### Reg No : 212223240122

```
import pandas as pd
import matplotlib.pyplot as plt
data=pd.read_csv("NSE-TATAGLOBAL11.csv")
data["Date"] = pd.to_datetime(data["Date"])
mean_value = data["Turnover (Lacs)"].mean()
print("Mean Price =", mean_value)
plt.figure(figsize=(8,5))
plt.plot(data["Date"], data["Turnover (Lacs)"])
plt.xlabel("Date")
plt.ylabel("Turnover")
plt.title("Time Series Plot")
plt.show()
```
# OUTPUT:

<img width="271" height="26" alt="Screenshot 2026-02-14 073332" src="https://github.com/user-attachments/assets/1220a4fb-bb87-454e-938f-57f1482f8fde" />

<img width="823" height="492" alt="Screenshot 2026-02-14 073344" src="https://github.com/user-attachments/assets/66b1cac7-9399-43fe-a2a3-f9ad6e6deeaf" />


# RESULT:
Thus we have created the python code for plotting the time series of given data.
