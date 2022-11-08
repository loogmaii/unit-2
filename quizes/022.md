# Quiz 22

A:

B:

## Code

```py
import random
random.seed(1234)
def produce(n,m,s):
    print(f'|       x        |            y(x)           |')
    for i in range(n):
        x = random.randint(0, 100)
        y = x ** (1 / 2 * (m / s) ** 2)
        roundedy = round(y, 2)
        print(f'|   {str(x).center(10)}   |         {str(roundedy).center(10)}        |')

sample = produce(n=5,m=3,s=2)
print(sample)
```

## Evidence

<sub>Fig.1 shows results of the program

## Truth table
  
<sub>Fig.2 shows the truth table

## Circuit

<sub>Fig.3 shows the boolean circuit for part B
