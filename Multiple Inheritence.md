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

    class optimus:
        def __init__(self, a, b):
            self.a = a
            self.b = b
        
    class megatron(optimus):
        def __init__(slef, a, b):
            super().__init__(a,b)
            print(a+b)
            print(a-b)
            print(a*b)
            
    num1 = int(input())
    num2 = int(input())

    obj = megatron(num1, num2)

## Output Example

<img width="1123" height="204" alt="image" src="https://github.com/user-attachments/assets/f8387a3b-1e1c-4f09-be79-ee5a531edcc0" />

##Result
The program executed successfully.
