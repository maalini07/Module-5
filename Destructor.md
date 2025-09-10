# Destructor in Python

This project demonstrates how to implement a **destructor** in Python using a simple class.

## 🚀 Overview

The program defines a class `Demo` with:

- A **constructor** `__init__` that initializes an instance variable and prints a message.
- A **destructor** `__del__` that prints a message when the object is destroyed.

## 🧠 Algorithm

1. Define a class named `Demo`.
2. Inside the class, define the `__init__` method:
   - Initialize an instance variable `status` with the value `"Alive"`.
   - Print the value of `status`.
3. Define the `__del__` method:
   - Print a message indicating the object is being destroyed.
4. Outside the class:
   - Create an instance of the `Demo` class.
   - Delete the object using the `del` keyword.
## Program
```
  class Demo:
     def __init__(self):
        self.status = "Alive"
     def __del__(self):
        print("The object no longer exists")
     
  obj = Demo()
  # The status has been initialized to Alive
  print(obj.status)
```

## 🧪 Output
<img width="658" height="166" alt="449879173-0c6c5a6d-34b3-48cf-bb8a-f0a859967cc3" src="https://github.com/user-attachments/assets/395d65b4-73b9-4e17-b410-f96ffc879629" />

## Result
Thus,the program has executed successfully.
