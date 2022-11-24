# Quiz 24

A: Create a program shows the graph of the parabola for 100 values of x in the interval -10 < x < 10  

B: Circuit for:
not(bit0 bit1 + not (bit0 + bit1)) 


## Code

```py
def produce():
    print(f'|       x        |            y(x)           |')
    x = []
    y = []
    st = -10
    for i in range(101):
        x.append(st)
        eq = 2 * (i + 5) ** 2
        y.append(eq)
        st += 0.2
        print(f'|   {str(x).center(10)}   |         {str(y).center(10)}        |')
    return x, y

x, y = produce()

from matplotlib import pyplot as plt
plt.style.use('ggplot')
plt.plot(x, y)
plt.plot(x, y, color = 'deeppink')
plt.xlabel("x")
plt.ylabel("f(x) = 2(x+5)^2")
plt.show()
```

## Evidence/Graph

<img width="633" alt="Screen Shot 2565-11-24 at 23 12 38" src="https://user-images.githubusercontent.com/111941936/203805083-e5253935-874d-4c62-ad4c-b0425073e095.png">

<sub>Fig.1 shows results of the program

## Circuit

![IMG_5589DBA19805-1](https://user-images.githubusercontent.com/111941936/203817589-a58aa404-10af-4006-87c4-a5f55dc89927.jpeg)
    
<sub>Fig.2 shows the boolean circuit for part B
