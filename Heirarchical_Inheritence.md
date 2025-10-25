# Hierarchical Inheritance in Python

This Python project demonstrates **Hierarchical Inheritance** using a base class `Details` and two derived classes `Employee` and `Patient`. The program collects and displays details for both employees and patients.

## 🎯 Aim

To write a Python program that uses **Hierarchical Inheritance** to input and display **Employee** and **Patient** details.

## 📘 Description

- **Base Class:** `Details`
  - Stores common attributes: `name`, `age`
  - Provides methods: `getName()`, `getAge()`

- **Derived Class 1:** `Employee`
  - Inherits from `Details`
  - Adds: `employee_id`, `department`
  - Method: `getEmployeeDetails()`

- **Derived Class 2:** `Patient`
  - Inherits from `Details`
  - Adds: `patient_id`, `disease`
  - Method: `getPatientDetails()`

## 🧠 Algorithm

1. Create base class `Details` with common attributes.
2. Create `Employee` class extending `Details`, adding employee-specific data.
3. Create `Patient` class extending `Details`, adding patient-specific data.
4. Get user input for employee and patient data.
5. Display collected information using class methods.

## Program

    class doctor:
        def __init__(self, id_no, name, g, hospital, dept):
            self.name = name
            self.id_no = id_no
            self.g = g
            self.hospital = hospital
            self.dept = dept
        
    class patient:
        def __init__(self, pid, pname, pg, phospital, pdept):
            self.pname = pname
            self.pid = pid
            self.pg = pg
            self.phospital = phospital
            self.pdept = pdept
        
    class display(doctor, patient):
        def __init__(self, id_no, name, g, hospital, dept, pid, pname, pg, phospital, pdept):
            doctor.__init__(self,id_no, name, g, hospital, dept)
            patient.__init__(self, pid, pname, pg, phospital, pdept)
            print("Doctor Object")
            print(f"Id:  {id_no}\nName:  {name}\nGender:  {g}\nHospital:  {hospital}\nDepartment:  {dept}\n")
            print("Patient Object")
            print(f"Id:  {pid}\nName:  {pname}\nGender:  {pg}\nHospital:  {phospital}\nDepartment:  {pdept}\n")
        
    id_no = int(input())
    name = input()
    g = input()
    hospital = input()
    dept = input()

    pid_no = int(input())
    pname = input() 
    pg = input()
    phospital = input()
    pdept = input()

    obj = display(id_no, name, g, hospital, dept, pid_no, pname, pg, phospital, pdept)

## Sample Output
<img width="1127" height="457" alt="image" src="https://github.com/user-attachments/assets/29750521-36b0-41c4-b9d5-3aa128a91df5" />

## Result
The program executed successfully.
