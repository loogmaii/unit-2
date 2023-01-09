# Quiz 32

A: Compare the data from sensor#9 and 10 with smoothing of 12 samples.

B: What are the three main operators used in boolean logic?

## Code

```py
import requests
from matplotlib import pyplot as plt
import numpy as np

req = requests.get('http://192.168.6.142/readings')
data = req.json()
readings = data["readings"][0]
T_9 = []
samples_9 = []
for red in readings:
    if red["sensor_id"]==9:
        T_9.append(red['value'])
T_10 = []
samples_10 = []
for r in readings:
    if r["sensor_id"]==10:
        T_10.append(r['value'])

print(T_9, T_10)

fig = plt.figure(figsize=(8,4))
plt.subplot(1,2,1)
plt.plot(T_9,samples_9, color="blue")
plt.plot(T_10,samples_10, color="pink")

mean = []
standard_dev = []
for s in range(0,len(T_9)):
    data = [T_9[s], T_10[s]]
    mean.append(np.mean(data))
    standard_dev.append(np.std(data))

plt.subplot(1,2,2)
plt.plot(mean, color="#003049")
plt.fill_between(T_9, T_10, alpha = .5, color="#caf0f8")

plt.show()
```

## Evidence

<sub>Fig.1 shows results of the program

<sub>Fig.2 shows the graph of the program

## Citations

<sub>Fig.3 shows the boolean circuit for part B
