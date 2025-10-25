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

    class Person:
        def __init__(self, name): 
            self.name = name

    class PersonDetails(Person):
        def __init__(self, name, age): 
            super().__init__(name) 
            self.age = age

    class PersonLocation(PersonDetails):
        def __init__(self, name, age, location): 
            super().__init__(name, age) 
            self.location = location

        def display(self):
            print(f"{self.name} {self.age} {self.location}")

    name = input()
    age = int(input())
    location = input()

    person = PersonLocation(name, age, location)
    person.display()  


## Sample Output

<img width="1129" height="204" alt="image" src="https://github.com/user-attachments/assets/1cd5649a-cd0f-4755-ab59-2b477ebe1358" />

## Result
The program executed successfully.
