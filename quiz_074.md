## Task
<img width="954" alt="Screenshot 2024-09-10 at 01 34 57" src="https://github.com/user-attachments/assets/f7c8196b-5213-4120-8253-fa8c4d55dc67">


```.py
def parity_check(message: str):
    num = 0
    for i in range(1, len(message)):
        if message[i] == '1':
            num += 1
    return num%2 == int(message[0])

print(parity_check('100111001011001110010110011100101'))
print(parity_check('011101111101110111110111001111'))
```

## Proof of work

<img width="1440" alt="Screenshot 2024-09-10 at 01 35 21" src="https://github.com/user-attachments/assets/ec1164e0-96be-442f-9ba6-92c4ac2684e7">

## Class work

Was not in class, so did it at home independantly
