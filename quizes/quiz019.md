# Quiz 19

create a function that changes the vowels in a string to numbers such as a = 4, e = 3, i = 1, o = 0 and space by _

## code

```py
def get_l3tt3r(msg:str):
    output = ''
    for letter in msg:
        if letter == 'i':
            output += '1'
        elif letter == 'a':
            output += '4'
        elif letter == 'e':
            output += '3'
        elif letter == 'o':
            output += '0'
        elif letter == ' ':
            output += '_'
        else:
            output += letter
    return output
```

## evidence

<img width="429" alt="Screen Shot 2565-10-28 at 15 18 59" src="https://user-images.githubusercontent.com/111941936/198516990-156c5142-b6d4-4d9b-a399-4ab6a44c86ac.png">

## boolean circuit

AB + not(B+C) + B(notC notA)
