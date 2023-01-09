# Quiz 28

A: Create a graph for the x, y data below:

data =  {
'x': [0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14, 15, 16, 17, 18, 19],
'y': [24, 1, 2, 25, 26, 21, 23, 34, 49, 2, 19, 32, 7, 17, 36, 7, 45, 28, 40, 46]
}  

Add a the item “title”:“quiz028” to the dictionary.


B: Convert the following rgb color to hex color : red=10, green=255, blue=255

## Code

```py
from matplotlib import pyplot as plt

data = {
    "x": [0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14, 15, 16, 17, 18, 19],
    "y": [24, 1, 2, 25, 26, 21, 23, 34, 49, 2, 19, 32, 7, 17, 36, 7, 45, 28, 40, 46],
    "title": "quiz028"
    }
print(data)
plt.plot(data["x"], data["y"], color = "deeppink")
plt.title(data["title"])
plt.show()
```

## Evidence

<img width="1240" alt="Screen Shot 2566-01-07 at 09 24 59" src="https://user-images.githubusercontent.com/111941936/211127374-9bb9dd7c-3625-4031-a29f-20bb3c418edd.png">

<sub>Fig.1 shows results of the program
  
<img width="620" alt="Screen Shot 2566-01-07 at 09 25 19" src="https://user-images.githubusercontent.com/111941936/211127389-04b112f2-38d0-4b0a-8c25-53589d17a34d.png">

<sub>Fig.2 shows graph of the program

## Part B
    
![E41F675A-A2D9-48D7-A004-4F7AB5C799E9](https://user-images.githubusercontent.com/111941936/211260060-13520585-5fe1-4e3b-8aff-ae9c5c13ff6f.jpg)    
    
<sub>Fig.3 shows results of part B
