# Exp.No:24  
## Multi-level Inheritance

---

### AIM  
To write a Python program to get the name, age, and ID of a person and display them using multilevel inheritance.

---

### ALGORITHM

1. Define the `Person` class:
   - Inside the `Person` class, define the `__init__` method (constructor) with two parameters: `name` and `age`.
   - Inside the `__init__` method, assign the `name` to `self.name` and `age` to `self.age`.

2. Define the `PersonDetails` class that inherits from the `Person` class:
   - Inside the `PersonDetails` class, define the `__init__` method (constructor) with three parameters: `name`, `age`, and `person_id`.
   - Inside the `__init__` method, call the `__init__` method of the `Person` class using `super()` to initialize `name` and `age`.
   - Assign `person_id` to `self.person_id`.

3. Define the `DisplayDetails` class that inherits from the `PersonDetails` class:
   - Inside the `DisplayDetails` class, define the `__init__` method (constructor) with three parameters: `name`, `age`, and `person_id`.
   - Inside the `__init__` method, call the `__init__` method of the `PersonDetails` class using `super()` to initialize `name`, `age`, and `person_id`.

4. Inside the `DisplayDetails` class, define the `show_details` method:
   - Inside the `show_details` method, return a formatted string with `self.name`, `self.age`, and `self.person_id`.

5. Prompt the user to enter `name` (string), `age` (integer), and `person_id` (integer).

6. Create an instance `person` of the `DisplayDetails` class, passing `name`, `age`, and `person_id` to the constructor.

7. Call the `show_details` method on the `person` object and print the result.

8. Terminate the program.

---

### PROGRAM

```
# Hybrid Inheritance
class vehicle:
    
    def __init__(self,model,mileage,price):
        self.price = price
        self.mileage = mileage
        self.model = model
        
    def show_details(self):
        print(f'Model : {self.model}')
        print(f'Price : {self.price}')
        print(f'Mileage : {self.mileage}')
                
class bike(vehicle):
    
    # Inherit Properties and Override
    def __init__(self,model,mileage,price,tyre,cc):
        super().__init__(model,mileage,price)
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
price=int(input())
tyre=int(input())
cc=int(input())

nam=input()
mil=int(input())
pri=int(input())
tyr=int(input())
cc1=int(input())
bajaj = bike(name,mile,price,tyre,cc)
tata = car(nam,mil,pri,tyr,cc1)

bajaj.show_details()
tata.show_details()

bajaj.rating()
tata.rating()

```

### OUTPUT
![image](https://github.com/user-attachments/assets/6e730fa1-9ec2-4607-b2fb-29f5ce69fdf3)

### RESULT
Thus the program Multi-level Inheritance have been executed and verified sucessfully.
