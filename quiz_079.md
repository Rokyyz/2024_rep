## Task
<img width="963" alt="Screenshot 2024-09-13 at 07 31 13" src="https://github.com/user-attachments/assets/78ada9df-4cb7-40c0-94c3-ccbb60fac4e7">


## Classwork

![CommSci 58](https://github.com/user-attachments/assets/aaf9dc45-f21b-4488-8d78-a39f71c8a2cd)

```.py

def calculate_parity_bit(msg):
    p = 0
    while (2 ** p) < (len(msg) + p + 1):
        p += 1
    return p
def hamming_code_full(msg):
    parity_count = calculate_parity_bit(msg)
    total_len = len(msg) + parity_count
    final_list = ['_'] * total_len
    j = 0
    for i in range(1, total_len + 1):
        if (i & (i - 1)) == 0:
            final_list[i - 1] = '-1'
        else:
            final_list[i - 1] = msg[j]
            j += 1
    for i in range(parity_count):
        parity_position = 2 ** i
        parity = 0
        for j in range(1, total_len + 1):
            if j & parity_position:
                if final_list[j - 1] != '-1':
                    parity ^= int(final_list[j - 1])
        final_list[parity_position - 1] = str(parity)

    return ''.join(final_list)

try1 = '1011'
print_full = hamming_code_full(try1)
print(f'full message: {print_full}')

try2 = '1111'
print_full = hamming_code_full(try2)
print(f'full message: {print_full}')

try3 = '1001'
print_full = hamming_code_full(try3)
print(f'full message: {print_full}')

```
## Proof of work
<img width="1393" alt="Screenshot 2024-09-13 at 07 30 25" src="https://github.com/user-attachments/assets/04267eb0-5d49-4591-8659-04d4a97d34c3">


## Proof of work
