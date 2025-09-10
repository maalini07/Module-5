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
```
class Details:
    def __init__(self, name, age):
        self.name = name
        self.age = age
    
    def getName(self):
        return self.name
    
    def getAge(self):
        return self.age
class Employee(Details):
    def __init__(self, name, age, employee_id, department):
        super().__init__(name, age)
        self.employee_id = employee_id
        self.department = department
    
    def getEmployeeDetails(self):
        print("\nEmployee Details:")
        print(f"Name: {self.getName()}")
        print(f"Age: {self.getAge()}")
        print(f"Employee ID: {self.employee_id}")
        print(f"Department: {self.department}")


class Patient(Details):
    def __init__(self, name, age, patient_id, disease):
        super().__init__(name, age)
        self.patient_id = patient_id
        self.disease = disease
    
    def getPatientDetails(self):
        print("\nPatient Details:")
        print(f"Name: {self.getName()}")
        print(f"Age: {self.getAge()}")
        print(f"Patient ID: {self.patient_id}")
        print(f"Disease: {self.disease}")
print("Enter Employee Details:")
emp_name = input("Name: ")
emp_age = int(input("Age: "))
emp_id = input("Employee ID: ")
emp_dept = input("Department: ")
print("\nEnter Patient Details:")
pat_name = input("Name: ")
pat_age = int(input("Age: "))
pat_id = input("Patient ID: ")
pat_disease = input("Disease: ")
employee = Employee(emp_name, emp_age, emp_id, emp_dept)
patient = Patient(pat_name, pat_age, pat_id, pat_disease)
employee.getEmployeeDetails()
patient.getPatientDetails()
````
## Sample Output
<img width="607" height="802" alt="449923774-3bf48904-705f-4ced-95b3-eeaa9be6ce7a" src="https://github.com/user-attachments/assets/a7993286-e86e-4e21-a803-bd86203087a7" />

## 🧪 Output
Thus, the program has executed successfully.

