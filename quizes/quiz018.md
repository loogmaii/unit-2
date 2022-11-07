# Quiz 18

create a function to help lily

## Code 

```py
#mine
def numberMatches(l,s):
    output = ''
    m = s // 20
    matches = l // m
    output = f'{matches} matches'
    return output

test1 = numberMatches(100,100)

#Dr Ruben's 
def numberMatches(l,s):
    lily_position = 0
    speed_m_per_s = s/100
    seconds_passed = 0
    matches = 0
    while lily_position < l:
        seconds_passed += 1
        # move lily
        lily_position += speed_m_per_s
        if seconds_passed ==5:
            matches == 1
            print(f'A match is lit. Lily is at {lily_position}')
            seconds_passed = 0
    return matches

test1 = numberMatches(100,100)
print(test1)
```

## Flowdiagram for Dr Ruben's code

![IMG_8E6FA9A869BA-1](https://user-images.githubusercontent.com/111941936/200209009-8d76d2ae-57e3-4e8d-a083-90088fc8ddf0.jpeg)

<sub>Fig.1 shows the flowchart for Dr Ruben's code

## Evidence

mine:

<img width="331" alt="Screen Shot 2565-10-26 at 11 37 56" src="https://user-images.githubusercontent.com/111941936/197921319-e68d8b57-deaf-46e9-a2b2-767a5dd142a8.png">

<sub>Fig.2 shows the results of my code
    
Dr Ruben's:

<img width="371" alt="Screen Shot 2565-10-26 at 11 36 38" src="https://user-images.githubusercontent.com/111941936/197921178-5325fdcc-8e1a-4ed8-b4a6-6b65f0520ab0.png">

<sub>Fig.3 shows the results of Dr Ruben's code
