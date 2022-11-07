# Quiz 19

A: create a function that changes the vowels in a string to numbers such as a = 4, e = 3, i = 1, o = 0 and space by _

|         Input msg:str         |          Output :str          |
|:-----------------------------:|:-----------------------------:|
|         “Hello World”         |         “H3ll0_W0rld”         |
|     “Why did I choose CS?”    |     “Why_d1d_1_ch00s3_CS?”    |
| “Remember the Figure Caption” | “R3m3mb3r_th3_F1gur3_C4pt10n” |

B: Boolean circuit for: AB + not(B+C) + B(notC notA)

## Code

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

## Evidence

<img width="429" alt="Screen Shot 2565-10-28 at 15 18 59" src="https://user-images.githubusercontent.com/111941936/198516990-156c5142-b6d4-4d9b-a399-4ab6a44c86ac.png">

<sub>Fig.1 shows results of the program

## boolean circuit

<sub>Fig.2 shows the boolean circuit for part B
