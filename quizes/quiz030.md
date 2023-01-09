# Quiz 30

A: Using the data in the learning Log (Item 21), create a graph with a smoothed version where the smoothing window is every 4 points.

B: When was the internet first created? Remember to add your sources

## Code

```py
from matplotlib import pyplot as plt

h = [57.0, 56.0, 57.0, 56.0, 55.0, 55.0, 54.0, 54.0, 54.0, 53.0, 53.0, 54.0, 53.0, 53.0, 52.0, 52.0, 51.0, 51.0,
         51.0, 50.0, 50.0, 49.0, 50.0, 49.0, 49.0, 48.0, 49.0, 49.0, 48.0, 48.0, 48.0, 49.0]
plt.style.use('ggplot')

x = [] #empty list
samples_per_window = 4
y = [] #smoothed version
for i in range(0,len(h),samples_per_window):
    data_in_window = h[i:i+samples_per_window]
    y.append(sum(data_in_window)/samples_per_window)
    x.append(i)

plt.plot(x, y, 'o-' )
plt.ylabel('Relative humidity')
plt.xlabel('samples')
plt.show()
```

## Evidence

<img width="1315" alt="Screen Shot 2566-01-07 at 09 33 39" src="https://user-images.githubusercontent.com/111941936/211127626-0f6b1c27-f074-4b4c-b3f8-8ecfb412b1df.png">

<sub>Fig.1 shows results of the program

<img width="625" alt="Screen Shot 2566-01-07 at 09 34 06" src="https://user-images.githubusercontent.com/111941936/211127639-fd171d7d-d32c-4470-8cd5-b8cc004609e6.png">

<sub>Fig.2 shows the graph of the program

## Part B
  
The internet was first created in January 1st, 1983[^1]
         
[^1]:“A Brief History of the Internet.” Usg.edu, 2023, www.usg.edu/galileo/skills/unit07/internet07_02.phtml#:~:text=January%201%2C%201983%20is%20considered,Protocol%20(TCP%2FIP).

‌
