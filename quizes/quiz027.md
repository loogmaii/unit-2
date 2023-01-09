# Quiz 27

A: Create a errorbar graph for the data below. You will need to calculate the mean and standard deviation first.

sensorA = [16, 24, 24, 9, 23, 26, 26, 23, 25, 14]  
sensorB = [2, 19, 25, 10, 11, 24, 17, 7, 24, 17]  
sensorC = [15, 11, 24, 21, 6, 2, 18, 27, 1, 16]  


B: Convert the following rgb color to hex color : red=250, green=100, blue=10

## Code

```py
from matplotlib import pyplot as plt
import numpy as np

plt.style.use('ggplot')

sensorA = [16, 24, 24, 9, 23, 26, 26, 23, 25, 14]
sensorB = [2, 19, 25, 10, 11, 24, 17, 7, 24, 17]
sensorC = [15, 11, 24, 21, 6, 2, 18, 27, 1, 16]

time = []
for i in range (len(sensorA)):
    time.append(i)

fig = plt.figure(figsize=(8,4))
plt.subplot(1,2,1)
plt.plot(time,sensorA, color="pink")
plt.plot(time,sensorB, color="violet")
plt.plot(time,sensorC, color="teal")
plt.ylabel("Samples")
plt.xlabel("Relative Humidity")

mean = []
standard_dev = []
min_v = []
max_v = []


for s in range(len(sensorA)):
    data = [sensorA[s], sensorB[s], sensorC[s]]
    mean.append(np.mean(data))
    min_v.append(min(data))
    max_v.append(max(data))
    standard_dev.append(np.std(data))

plt.subplot(1,2,2)
plt.plot(time, mean, color="teal")
plt.fill_between(time, min_v, max_v, alpha = .5, color="#caf0f8")
plt.errorbar(time, mean,standard_dev, fmt="o", color="#0077b6")
plt.show()

```

## Evidence

<img width="1401" alt="Screen Shot 2566-01-07 at 09 21 40" src="https://user-images.githubusercontent.com/111941936/211127277-4fcb0670-0d96-4ac9-bde6-044eee8771d0.png">

<sub>Fig.1 shows results of the program
 
<img width="787" alt="Screen Shot 2566-01-07 at 09 22 06" src="https://user-images.githubusercontent.com/111941936/211127287-1c2fd076-5c05-4828-b2d6-5657b18dcfd1.png">

<sub>Fig.2 shows graph of the program

## Part B
    
![D46D30F8-3BEA-4EC5-A28D-8B9ECDB76C2B](https://user-images.githubusercontent.com/111941936/211258279-7a8f4fea-f593-4cd4-be51-7ebe47c57506.jpg)  
    
<sub>Fig.3 shows results of part B
