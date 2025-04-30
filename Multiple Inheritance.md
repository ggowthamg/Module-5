# Exp.No:23  
## Multiple Inheritance

---

### AIM  
To write a Python program to get the name, attendance, and ID of a student and check if they are eligible for the next module using multiple inheritance. If attendance > 80, the student is eligible; otherwise, not eligible.

---

### ALGORITHM

1. Define the `Student` class.
2. Inside the `Student` class, define the `__init__` method (constructor). The `__init__` method accepts two parameters: `name` and `student_id`.
    - Inside the `__init__` method: Assign the value of `name` to `self.name` and `student_id` to `self.student_id`.
3. Define the `get_student_info` method inside the `Student` class:
    - This method should return a string formatted with `self.name` and `self.student_id`.
4. Define the `Attendance` class, which inherits from the `Student` class.
5. Inside the `Attendance` class, define the `__init__` method (constructor).
    - The `__init__` method accepts three parameters: `name`, `student_id`, and `attendance`.
    - Inside the `__init__` method: Call the parent class constructor `super().__init__(name, student_id)` to initialize `name` and `student_id`. Assign the value of `attendance` to `self.attendance`.
6. Define the `check_eligibility` method inside the `Attendance` class:
    - If `self.attendance` is greater than 80, return a formatted string indicating the student is eligible for the module exam.
    - Otherwise, return a formatted string indicating the student is not eligible for the module exam.
7. Prompt the user to enter the `name` (as a string), `student_id` (as an integer), and `attendance` (as an integer).
8. Create an instance `student` of the `Attendance` class, passing the entered `name`, `student_id`, and `attendance` to the constructor.
9. Call the `check_eligibility` method on the `student` object and print the result.
10. Terminate the program.

---

### PROGRAM

```
# Hybrid Inheritance
class vehicle:
    
    def __init__(self,model,mileage):
        
        self.mileage = mileage
        self.model = model
        
    def show_details(self):
        print(f'Model : {self.model}')
       
        print(f'Mileage : {self.mileage}')
                
class bike(vehicle):
    
    # Inherit Properties and Override
    def __init__(self,model,mileage,tyre,cc):
        super().__init__(model,mileage)
        self.cc = cc
        self.tyre = tyre
    
    # Inherit Behavior and Override
    def show_details(self):
        super().show_details()
        print(f'CC : {self.cc}')
        print(f'Tyres : {self.tyre}')
    
    # Method of Derived Class
    def rating(self):
        print('4 star')
        

class car(bike,vehicle):
    
    def rating(self):
        print('5 star')

name=input()
mile=int(input())

tyre=int(input())
cc=int(input())

nam=input()
mil=int(input())

tyr=int(input())
cc1=int(input())
bajaj = bike(name,mile,tyre,cc)
tata = car(nam,mil,tyr,cc1)

bajaj.show_details()
tata.show_details()

bajaj.rating()
tata.rating()
```

### OUTPUT
![image](https://github.com/user-attachments/assets/7846b2a1-ebff-442c-b704-32eeff764b88)


### RESULT
Thus the program Multiple Inheritance have been executed and verified sucessfully.




