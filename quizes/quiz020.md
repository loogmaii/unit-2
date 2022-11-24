# Quiz 20

A: Create a function that produces the table of Truth for 3 inputs

B: Truth table and circuit for: Light = S1S2+(S2+S3(notS1))S1 

## Code

```py
def get_truth():
    print(f"| A | B | C |")
    for i in range(8):
        a = i // 4
        b = (i % 4) // 2
        c = i % 2
        print(f"| {a} | {b} | {c} |")

table = get_truth()
print(table)
```

## Evidence

<img width="362" alt="Screen Shot 2565-11-03 at 08 23 45" src="https://user-images.githubusercontent.com/111941936/199620717-db3072b0-f0ea-4621-9f6a-035b0eddc1cd.png">

<sub>Fig.1 shows results of the program

## Truth table
   
![IMG_263385BC8163-1](https://user-images.githubusercontent.com/111941936/203371328-3bf6097a-b3dd-4aeb-b5e4-45541c82b44c.jpeg)
  
<sub>Fig.2 shows the truth table

## Circuit
  
![IMG_1A9917C700B3-1](https://user-images.githubusercontent.com/111941936/203816982-dfbfc434-bfc2-4d94-9939-a3b03290a041.jpeg)
    
<sub>Fig.3 shows the boolean circuit for part B
