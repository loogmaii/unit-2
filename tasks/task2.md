# Task 2

<img width="987" alt="Screen Shot 2565-11-11 at 03 14 03" src="https://user-images.githubusercontent.com/111941936/201174313-1f89e669-193d-4eb2-a4ea-79f8fdeaecc9.png">

Fig. 1 System diagram for the proposed binary counter. The diagram shows the two main computer systems, the server (left: laptop) and client (right: microcontroller). The server implements a 3 bits binary counter (0 to 7 in decimal) using a function and sends the state (on/off) for the three LEDs in the client.

# Code 

```py
from pyfirmata import Arduino
import time

def validate_int_input(msg:str)->int:
    number=input(msg)
    while not number.isdigit():
        number = input( f'error, {msg}')
    return int(number)

board = Arduino('/dev/cu.usbserial-1420')
print("Communication succesfully started")

while True:
    n = validate_int_input(input("Please input an integer: "))
    i = n
    a = i // 4
    b = (i % 4) // 2
    c = i % 2
    board.digital[12].write(a)
    board.digital[9].write(b)
    board.digital[5].write(c)
    time.sleep(0.5)
``` 

