# Quiz 29

A: Create a function that receives a dictionary with letters in the alphabet as keys and a string. The functions returns the dictionary with a count as value for the occurrence of each letter:

|               Input lexicon:dict, msg:str               |            Output :str           |
|:-------------------------------------------------------:|:--------------------------------:|
|            {‘w’:0,‘l’:0,‘c’:0}, “hello world”           |       {‘w’:1, ‘l’:3, ‘c’:0}      |
| {‘a’:0,‘e’:0,‘i’:0,‘o’:0,‘u’:0}, “Why did I choose CS?” | {‘a’:0,‘e’:1,‘i’:1,‘o’:2,‘u’:0}, |

case1 = count_letters(my_dict, msg)
print(case1)


B: How many different colors could you represent in a 6 bit computer? 

## Code

```py
def count_letters(lexicon,msg):
    for letter in msg:
        if letter in lexicon.keys():
            lexicon[letter] += 1
    return lexicon

w_l_c = {'w':0,'l':0,'c':0}
case1 = count_letters(w_l_c,'hello world')
print(case1)

vowels = {'a':0,'e':0,'i':0,'o':0,'u':0}
case2 = count_letters(vowels,'Why did I choose CS?')
print(case2)
```

## Evidence

<img width="493" alt="Screen Shot 2566-01-07 at 09 29 30" src="https://user-images.githubusercontent.com/111941936/211127514-2e45d3f2-942e-4f30-a02b-433de2b8658f.png">

<sub>Fig.1 shows results of the program

## Part B
  
64 colors can be represented in a 6 bit computer[^1]
    
[^1]:“Concept of Bits per Pixel.” Tutorialspoint.com, 2023, www.tutorialspoint.com/dip/concept_of_bits_per_pixel.htm. 
