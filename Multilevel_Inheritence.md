# Multilevel Inheritance Example in Python

This Python project demonstrates the concept of **Multilevel Inheritance** to collect and display the **name**, **age**, and **location** of a person.

## 🎯 Aim

To write a Python program that uses multilevel inheritance to get and display a person’s name, age, and location.

## 🧠 Algorithm

1. **Parent Class**  
   - `__init__(name)` initializes the `name` attribute.  
   - `getName()` returns the `name`.

2. **Child Class (inherits Parent)**  
   - `__init__(name, age)` initializes `name` using `super()` and adds `age`.  
   - `getAge()` returns the `age`.

3. **Grandchild Class (inherits Child)**  
   - `__init__(name, age, location)` initializes `name` and `age` using `super()` and adds `location`.  
   - `getLocation()` returns the `location`.

4. **Input & Output**  
   - Take user input for name, age, and location.  
   - Create an instance of `Grandchild`.  
   - Print all details using class methods.

## Program
```
  class Parent:
     def __init__(self,name):
       self.name = name
     def getName(self):
       return self.name
  class Child(Parent):
     def __init__(self,name,age):
       Parent.__init__(self,name)
       self.age = age
     def getAge(self):
       return self.age
  class Grandchild(Child):
     def __init__(self,name,age,location):
       Child.__init__(self,name,age)
       self.location=location
     def getLocation(self):
       return self.location
  name=input()
  age=int(input())
  loc=input()
  gc = Grandchild(name,age,loc)
  print(gc.getName(), gc.getAge(), gc.getLocation())
```

## Sample Output
<img width="583" height="195" alt="449924900-97b138fe-0c84-4d6e-9479-02e0a2d6739f" src="https://github.com/user-attachments/assets/f6495727-7a02-46d3-8b96-ccbd0599b0d4" />

## 🧪 Output
Thus, the program has executed successfully
