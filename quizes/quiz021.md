# Quiz 21

A: Using the function that produces the table of Truth for 3 inputs, add a column for the boolean equation

AB+(not B)+(notB C)

B: X = ZW ⨁ (Z ⨁ Y(not W)) 

## Code

```py
def get_truth():
    print(f"| A | B | C | AB + not B + not CB |")
    for i in range(8):
        a = i // 4
        b = (i % 4) // 2
        bb = not b
        c = i % 2
        n = c * b
        m = not n
        d = a * b + bb + m
        print(f"| {a} | {b} | {c} |          {d}          |")

table = get_truth()
print(table)
```

## Evidence

<img width="599" alt="Screen Shot 2565-11-11 at 03 07 55" src="https://user-images.githubusercontent.com/111941936/201173205-796eaa20-e9aa-4c19-88ee-5e4dd6144d9d.png">

<sub>Fig.1 shows results of the program

## Truth table
    
![IMG_C999407013CD-1](https://user-images.githubusercontent.com/111941936/203800100-635c9331-cfc6-4bff-aba6-e57b5ac83740.jpeg)
  
<sub>Fig.2 shows the truth table

## Circuit

![IMG_59C6CA3DE935-1](https://user-images.githubusercontent.com/111941936/203800281-dff3621f-733d-4832-8a4d-0d28e25f74a2.jpeg)
  
<sub>Fig.3 shows the boolean circuit for part B

