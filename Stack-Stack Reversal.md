# # Stack-Stack Reversal Program 🔁

This Python program demonstrates how to reverse the values in a stack using basic stack operations like push and pop.

## 🎯 Aim

To write a Python program that reverses the values in a stack using standard stack operations.

## 📋 Algorithm

1. Create an empty stack.
2. Read an integer `n` from the user (number of elements to push).
3. Loop `n` times:
   - Read an integer from the user.
   - Push it onto the stack.
4. Create an empty list called `reverse`.
5. While the stack is not empty:
   - Pop the top element.
   - Append it to `reverse`.
6. Print the reversed list.


### Program:
~~~
def reverse_stack(stack):
    reversed_stack = []
    while stack:
        reversed_stack.append(stack.pop())
    return reversed_stack
stack = []
n = int(input("Enter the number of elements in the stack: "))
for i in range(n):
    value = input(f"Enter element {i + 1}: ")
    stack.append(value) 
print("\nOriginal Stack (Top to Bottom):")
print(stack[::-1]) 
stack = reverse_stack(stack)
print("\nReversed Stack (Top to Bottom):")
print(stack[::-1])
~~~

## 🧪 Sample Input and Output
![442495057-72d011b8-d294-46b1-a15a-85581aee471d](https://github.com/user-attachments/assets/de43e38f-3cbb-4c20-a833-b62ab5ce988a)

## Result
Thus the program has been executed successfully.
