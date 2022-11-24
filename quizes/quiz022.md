# Quiz 22

A: Create a program that produces n random values from the equation below, where m and s are the other inputs of the function

B: Proof that : A (A + B) = A 

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

<img width="778" alt="Screen Shot 2565-11-08 at 13 45 38" src="https://user-images.githubusercontent.com/111941936/200477272-0c04f26e-0efc-4b25-b729-b75969810858.png">

<sub>Fig.1 shows results of the program

## Truth table
    
![IMG_457A8D8DDFB1-1](https://user-images.githubusercontent.com/111941936/203801694-3c447850-b32a-4b92-bdd3-413337b8cf1d.jpeg)
 
<sub>Fig.2 shows the truth table that proves A (A + B) = A


    
