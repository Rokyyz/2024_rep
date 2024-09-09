## Task

<img width="970" alt="Screenshot 2024-09-10 at 01 42 29" src="https://github.com/user-attachments/assets/cc2743aa-1f63-4f6e-9c67-2dd790c46fb7">

## Classwork
![CommSci 56](https://github.com/user-attachments/assets/43c27aa8-19fb-4256-8a4c-6a7b85f8da52)


```.py
def get_equation(k,n,P):
    p_list = []
    for i in range(0,k+n):
        if i&(2**(P-1)) != 0:
            p_list.append(i-1)
    return p_list

equations = [get_equation(3,4,i) for i in range(1,4)]
print(equations)
```

## Proof of work
<img width="1440" alt="Screenshot 2024-09-10 at 01 43 03" src="https://github.com/user-attachments/assets/b61de151-ebf4-4651-97ec-5d2b22b874ce">
