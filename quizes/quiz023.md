# Quiz 23

A: Create a program that produces the graph for the function in Quiz #22  

B: Truth table for:
A(A ⊕ B)  


## Code

```py
import random
random.seed(1234)
def produce(n:int,m:int,s:int):
    print(f'|       x        |            y(x)           |')
    x_out = []
    y_out = []
    for i in range(n):
        x = random.randint(0, 100)
        x_out.append(x)
        y = x ** (1 / 2 * (m / s) ** 2)
        y_out.append(y)
        y_str = f'{y:.2f}'
        print(f'|   {str(x).center(10)}   |         {str(y_str).center(10)}        |')

    return y_out, x_out

from matplotlib import pyplot as plt

data_y, data_x = produce(n=10, m=3, s=2)
plt.plot(data_x, data_y, color="red", marker="+")
plt.xlabel("variable x")
plt.ylabel("$y=x^{1/2(m/s)^2}$")
plt.title('Equation from quiz 22')
plt.show()
```

## Evidence/Graph

<img width="633" alt="Screen Shot 2565-11-24 at 23 03 04" src="https://user-images.githubusercontent.com/111941936/203803004-4e0305e5-a942-4562-81b4-aa7ad0090f88.png">

<sub>Fig.1 shows results of the program
  

## Truth table
  
![IMG_D1363E6BFB33-1](https://user-images.githubusercontent.com/111941936/203803488-45fac0fd-d8c5-4693-84df-84b692159327.jpeg)  
  
<sub>Fig.2 shows the truth table
