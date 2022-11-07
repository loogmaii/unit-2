# Quiz 17

create a function that produces the average word length of the input list

|     Input  given :list     | Output :int |
|:--------------------------:|:-----------:|
|      [“hello”,“main”]      |     4.5     |
|  [“Peru”,“France”,“Nepal”] |     5.0     |
| [“Computer Science”,“Art”] |     9.5     |
|       [“one”, “two”]       |     3.0     |

## Code

```py
def averagelength(words):
    counts = 0
    for letter in words:
        counts += len(letter)
    average = counts/len(words)
    return average
```

## Evidence

<img width="486" alt="Screen Shot 2565-11-07 at 09 55 47" src="https://user-images.githubusercontent.com/111941936/200205974-fbbda42f-5267-42e9-ad0d-b2571bb539a1.png">
