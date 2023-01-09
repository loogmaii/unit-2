# Quiz 31

A:  Connect to the server and download the recordings data. From the data, build a linear model between t=610 and t=800 

## Code

```py
import requests
from matplotlib import pyplot as plt
import numpy as np

req = requests.get('http://192.168.6.142/readings')
data = req.json()
readings = data["readings"][0]
T = []
samples = []
for samples in readings:
    if samples["sensor_id"]==1:
        T.append(samples['value'])

temp_afternoon_mon=T[610:800]
x_mon = []
for i in range(len(temp_afternoon_mon)):
    x_mon.append(i)
#lineal model y=m*x+b
m,b = np.polyfit(x_mon, temp_afternoon_mon, 1)
y_lineal = []
x_lineal = [0, x_mon[-1]]
for i in x_lineal: #[-1] means the last value
    y_lineal.append(m*i+b)

#quadratic model: y = ax^2+b
p0, p1, p2 = np.polyfit(x_mon, temp_afternoon_mon, 2)
y_quad = []
for i in x_mon:
    y_quad.append(p0*(i**2) + p1*i +p2)

plt.plot(x_lineal, y_lineal, color='black')
plt.plot(x_mon, y_quad, color = 'blue')

plt.scatter(x_mon, temp_afternoon_mon)
plt.show()
```

## Evidence

<sub>Fig.1 shows results of the program

<sub>Fig.2 shows graph of the program
