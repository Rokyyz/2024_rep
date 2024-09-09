## Task

<img width="963" alt="Screenshot 2024-09-10 at 01 36 05" src="https://github.com/user-attachments/assets/e664b251-f729-4014-b9bc-b22f2f9dd8f0">

## Classwork

![CommSci 54](https://github.com/user-attachments/assets/d805098b-89b2-4310-a606-e2978644325d)

version 1 that produced the graph but did not give output of k
```.py
import numpy as np
import matplotlib.pyplot as plt

def parity(n):
    k=1
    while not 2**k >= n+k+1:
        k+=1
    return n/(k+n)

x = []
y = []
for i in range (1, 1001):
    x.append(i)
    y.append(parity(i)/i+parity(i))

plt.plot(x, y)
plt.figure(figsize=(10, 6))
plt.plot(x, y, color='red')
plt.xlabel('Length of the message', fontsize=12)
plt.ylabel('Efficiency', fontsize=12)
plt.title('Hamming Code efficiency', fontsize=14)
plt.grid(True)
plt.show()

```


## Proof of work
<img width="1440" alt="Screenshot 2024-09-10 at 01 37 19" src="https://github.com/user-attachments/assets/8536e561-5126-424a-b34b-80212dec48b9">


version that gives k
```.py
def get_k(n):
    k=1
    while not 2**k >= n+k+1:
        k+=1
    return k

x = get_k(4)
print(x)

```
## 2nd proof for 2nd version
<img width="1440" alt="Screenshot 2024-09-10 at 01 38 20" src="https://github.com/user-attachments/assets/eb700c38-5c29-4adb-8aec-de4793a5e5d5">

