# Exp.No:25  
## Hierarchical Inheritance

---

### AIM  
To write a Python program to get the employee and doctor details and display them using hierarchical inheritance. Create a parent (base) class named `Details` and two child (derived) classes named `Employee` and `Doctor`.

---

### ALGORITHM

1. **Begin the program.**
2. **Create a class Details** with an `__init__` method to initialize three attributes: `id`, `name`, and `gender`.
3. **Define a method display_details()** to print the values of `id`, `name`, and `gender`.
4. **Create a class Employee** that inherits from the `Details` class. 
   - Add two additional attributes: `company` and `department`.
   - Override the `display_details()` method to print the employee-specific attributes (`company` and `department`) along with the inherited details.
5. **Create a class Doctor** that also inherits from the `Details` class. 
   - Add two additional attributes: `hospital` and `department`.
   - Override the `display_details()` method to print the doctor-specific attributes (`hospital` and `department`) along with the inherited details.
6. **Accept input** for employee and doctor details.
7. **Create objects of Employee and Doctor** using the input.
8. **Call the `display_details()` method** for both objects to print the details.
9. **Terminate the program.**

---

### PROGRAM
```
class Doctor:
    def __init__(self ,a,b,c,d,e,a1,a2,a3,a4,a5):
        self.a=a
        self.b=b
        self.c=c
        self.d=d
        self.e=e
        self.a1=a1
        self.a2=a2
        self.a3=a3
        self.a4=a4
        self.a5=a5
        
    def display(self):
        print(f"Doctor Object\nId:  {self.a}\nName:  {self.b}\nGender:  {self.c}\nHospital:  {self.d}")
        print(f"Department:  {self.e}\n")
        print(f"Patient Object\nId:  {self.a1}\nName:  {self.a2}\nGender:  {self.a3}\nHospital:  {self.a4}")
        print(f"Department:  {a5}")
        
a=int(input())
b=input()
c=input()
d=input()
e=input()
a1=int(input())
a2=input()
a3=input()
a4=input()
a5=input()
Doctor=Doctor(a,b,c,d,e,a1,a2,a3,a4,a5)
Doctor.display()

```

### OUTPUT  
![image](https://github.com/user-attachments/assets/40b11d0c-fa74-4858-b8f6-27f4ee1b349a)


### RESULT
Thus the program Hierarchical Inheritance have been executed and verified sucessfully.

