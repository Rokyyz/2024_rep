## Task

<img width="966" alt="Screenshot 2024-09-10 at 00 57 24" src="https://github.com/user-attachments/assets/93e32555-5958-46ed-9a98-0c65414b6b9c">


```.py
def error_check(binary:str):
    num_ones = 0
    for bit in binary:
        if bit == '1':
            num_ones += 1
    return num_ones % 2 != 0


def correct_error(binary_message: str):
    length = len(binary_message) // 3
    original = binary_message[:length]
    copy1 = binary_message[length:2 * length]
    copy2 = binary_message[2 * length:]

    corrected_message = ""
    for i in range(length):
        bit_count = {'0': 0,'1': 0}
        bit_count[original[i]] += 1
        bit_count[copy1[i]] += 1
        bit_count[copy2[i]] += 1

        if bit_count['1'] > bit_count['0']:
            corrected_message += '1'
        else:
            corrected_message += '0'

    return corrected_message
binary_message1 = '100111001011001110010110011100101'
binary_message2 = '011101111101110111110111001111'

if error_check(binary_message1):
    print("Error detected in binary_message1. Corrected message:", correct_error(binary_message1))
else:
    print("No error detected in binary_message1:", binary_message1)

if error_check(binary_message2):
    print("Error detected in binary_message2. Corrected message:", correct_error(binary_message2))
else:
    print("No error detected in binary_message2:", binary_message2)
```

## Proof of work!
<img width="583" alt="Screenshot 2024-09-10 at 01 30 58" src="https://github.com/user-attachments/assets/92d258f2-a7cd-4d62-8556-41566e9fcdde">


## Class work

[CommSci 53](https://github.com/user-attachments/assets/8f6d03bf-0224-4055-b376-1c969bac3b5e)
