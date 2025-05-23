# Stack Implementation Using `LifoQueue` (Max Size 7) 🔄

This Python program demonstrates a stack implemented using the `LifoQueue` class from the `queue` module. It allows up to 7 elements, checks if the stack is full, and then prints the elements in reverse (LIFO) order.

## 🎯 Aim

To create a Python program that:
- Implements a stack using `LifoQueue` with a maximum size of 7
- Adds user-inputted values to the stack
- Checks whether the stack is full
- Prints the stack elements in reverse order (LIFO)

## 📋 Algorithm

1. Import the `LifoQueue` class from the `queue` module.
2. Create a stack with a maximum size of 7.
3. Read the number of elements (`n`) to be added to the stack.
4. Loop `n` times:
   - Read a value from the user.
   - Use `put()` to push it onto the stack if it's not full.
5. Use `full()` to check if the stack is full and print the result.
6. Use `get()` repeatedly to pop and print elements in reverse order.

## Program
~~~
from queue import LifoQueue
stack = LifoQueue(maxsize=7)
print("Enter up to 7 elements to push onto the stack:")
for i in range(7):
    value = input(f"Enter value {i + 1} (or press Enter to stop): ")
    if value == "":
        break
    stack.put(value)
if stack.full():
    print("The stack is full.")
else:
    print(f"The stack is not full. Current size: {stack.qsize()}")
print("\nStack elements in LIFO order:")
while not stack.empty():
    print(stack.get())
~~~
## 🧪 Sample Input and Output
![442494873-44f17f4e-c9c0-4720-89ad-8f3acdc03737](https://github.com/user-attachments/assets/e4686c9d-6721-45fe-918a-efea4c02f8ba)

## Result:
Thus the program has been executed successfully.
