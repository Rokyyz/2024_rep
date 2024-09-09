## Task
<img width="968" alt="Screenshot 2024-09-10 at 01 45 14" src="https://github.com/user-attachments/assets/5ab2427f-e347-4f76-ae74-4f2b00037dc9">


## Classwork

![CommSci 57](https://github.com/user-attachments/assets/abb94f3e-92a9-4694-96d7-5b94cb970a6c)


```.py
from quiz_75_version_2 import get_k
from quiz_076 import positions

def template(msg):
    k = get_k(len(msg))
    positions_all = positions(k)
    x = 0
    total_msg=[]
    for i in range(0, k+len(msg)):
        total_msg.append(-1)
        if i not in positions_all:
            total_msg[i] = msg[x]
            x+=1
    return total_msg
print(template('1011'))



```

## Proof of work

<img width="1440" alt="Screenshot 2024-09-10 at 01 44 45" src="https://github.com/user-attachments/assets/2e5afb94-db91-47f1-af72-a0dc437686a8">
