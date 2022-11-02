# Quiz 20

A: Create a function that produces the table of Truth for 3 inputs

B: Truth table and circuit for: Light = S1S2+(S2+S3(notS1))S1 

## code

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

## evidence

<img width="362" alt="Screen Shot 2565-11-03 at 08 23 45" src="https://user-images.githubusercontent.com/111941936/199620717-db3072b0-f0ea-4621-9f6a-035b0eddc1cd.png">

## Truth table

## Circuit
