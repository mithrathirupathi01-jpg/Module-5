# Arithmetic Operations Using Multiple Inheritance in Python

This Python program demonstrates **multiple inheritance** by performing basic arithmetic operations — Addition, Subtraction, and Division — using three classes.

## 🎯 Aim

To write a Python program to calculate **Add, Sub & Division** using **Multiple Inheritance**.

## 🧠 Algorithm

1. **Define `Calculation1` class**
   - Contains `Summation(a, b)` method to return the sum of two numbers.
2. **Define `Calculation2` class**
   - Contains `Subtraction(a, b)` method to return the difference of two numbers.
3. **Define `Derived` class**
   - Inherits from both `Calculation1` and `Calculation2`.
   - Contains `Division(a, b)` method to return the division result.
4. **Input**
   - Prompt the user to enter two numbers.
5. **Process**
   - Create an object of the `Derived` class.
   - Call `Summation`, `Subtraction`, and `Division` methods.
6. **Output**
   - Display the results of the three operations.

## 💻 Program 
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
## Output Example
<img width="512" height="151" alt="image" src="https://github.com/user-attachments/assets/24006bed-018c-4aa3-9917-2956c81ce5f4" />

## Result
Thus the program that uses multilevel inheritance to get and display a person’s name, age, and location executed successfully.


