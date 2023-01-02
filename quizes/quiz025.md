# Quiz 25

A: Create a program shows the graph of the function below for 100 values of x in the interval -10 < x < 10 

B: Convert to decimal: FFA5


## Code

```py
from matplotlib import pyplot as plt

def v_graph():
    x_ax = []
    y_ax = []
    st = -11
    for i in range(21):
        st += 1
        y = abs(st)
        x_ax.append(st)
        y_ax.append(y)
    return x_ax, y_ax

x_ax, y_ax = v_graph()
plt.plot(x_ax, y_ax)
plt.plot(x_ax, y_ax, color="teal")
plt.xlabel("x")
plt.ylabel("f(x) = |x|")
plt.show()
```

## Evidence

<img width="529" alt="Screen Shot 2566-01-02 at 21 20 10" src="https://user-images.githubusercontent.com/111941936/210243657-e5faa94f-e07a-4caa-a07b-3be08d5132db.png">


<sub>Fig.1 shows graph of the program

<img width="1190" alt="Screen Shot 2566-01-02 at 21 18 16" src="https://user-images.githubusercontent.com/111941936/210243403-c0fa74d6-9064-4647-9685-83d84061a07e.png">

<sub>Fig.2 shows results of the program

## Part B
