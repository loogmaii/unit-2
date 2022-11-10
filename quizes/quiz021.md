# Quiz 21

A: Using the function that produces the table of Truth for 3 inputs, add a column for the boolean equation

AB+(not B)+(notB C)

B: X = ZW ⨁ (Z ⨁ Y(not W)) 

## code

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

## Truth table

## Circuit
