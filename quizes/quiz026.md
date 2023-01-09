# Quiz 26

A:Create a program that ① show the graph and ②create a linear (H_model = m*h+b) for the data below:

h = [57.0, 56.0, 57.0, 56.0, 55.0, 55.0, 54.0, 54.0, 54.0, 53.0, 53.0, 54.0, 53.0, 53.0, 52.0, 52.0, 51.0, 51.0, 51.0, 50.0, 50.0, 49.0, 50.0, 49.0, 49.0, 48.0, 49.0, 49.0, 48.0, 48.0, 48.0, 49.0]   ＃32values

Where h is relative humidity (%)

B: Convert the following color in hex to rgb : #e6e627

## Code

```py
from matplotlib import pyplot as plt
import numpy as np

x = []
h = [57.0, 56.0, 57.0, 56.0, 55.0, 55.0, 54.0, 54.0, 54.0, 53.0, 53.0, 54.0, 53.0, 53.0, 52.0, 52.0, 51.0, 51.0,
         51.0, 50.0, 50.0, 49.0, 50.0, 49.0, 49.0, 48.0, 49.0, 49.0, 48.0, 48.0, 48.0, 49.0]
for i in range(1,33):
    x.append(i)

plt.scatter(x, h, color="violet")
plt.xlabel("samples")
plt.ylabel("relative humidity %")


m,b = np.polyfit(x, h, 1)
print(f"Linear equation is y ={m:.2f}x+({b:.2f})")
x_model = [1, 33]
y_model = []
for i in x_model:
    y_model.append(m * i + b)

x_13 = 13
y_pred_51 = m * x_13 +b
print(f"y = m * i + b")
plt.plot(x_13, y_pred_51, "b*", markersize = 20)
plt.text(15, 53, f"y = m * i + b")

plt.plot(x_model, y_model, color = "teal")
plt.title("Humidity on Campus")
plt.show()
```

## Evidence

<img width="1399" alt="Screen Shot 2566-01-07 at 09 13 46" src="https://user-images.githubusercontent.com/111941936/211126989-e0eaa4ae-5476-447b-9fc2-71fd2fe4bc82.png">

<sub>Fig.1 shows results of the program
 
<img width="622" alt="Screen Shot 2566-01-07 at 09 14 20" src="https://user-images.githubusercontent.com/111941936/211127012-74640aa2-c187-4a4f-993e-3ed5f5bf8b28.png">

<sub>Fig.2 shows graph of the program

## Part B
  ![CEDC0C86-A6D7-4353-97D4-A467D05BFB34](https://user-images.githubusercontent.com/111941936/211254607-3276d061-6adf-49e1-a146-f68ad3ee26b2.jpg)
         

         
         
<sub>Fig.3 shows results of part B
