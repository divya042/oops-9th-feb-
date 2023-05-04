```python

```


```python
1. create a vehicle class with an init method having instance variable as name_of_vehicle ,max_speed and average_of_vehicle.

Ans-
    class vehicle:
        def __init__(self , name_of_vehicle ,max_speed, average_of_vehicle):
            self.name_of_vehicle = name_of_vehicle
            self.max_speed = max_speed
            self.average_of_vehicle = average_of_vehicle
            
            car = vehicle("car",180,29)
            print("Name of vehicle":,cae.name_of_vehicle)
            print("Max speed":,car.max_speed)
            print("Averageof vehicle:",car.average_of_vehicle)
            
        output-
              Name of vehicle: car
              Max speed: 180
                Average of vehicle:20
            
```


      Cell In[2], line 1
        1. create a vehicle class with an init method having instance variable as name_of_vehicle ,max_speed and average_of_vehicle.
           ^
    SyntaxError: invalid syntax




```python
2. create a child class carfrom the vehicle classcreated in Que 1.which will inherit the vehicle class.
create a method named seating_capacity which takes capacity as an argument and returns the name of the vehicle and its 
seating capacity.

Ana- class car(vehicle): def init(self,name,make,model,year,weight):self.name = name self.make = make self.model=model
      self.year =year.self.weight = weight
         
class car(vehicle):
    def __init__(self, name,make,model,year,weight,num_doors):
    vehicle,__init__(self,name,make,model,year,weight)
    self.num_doors
    
    def seating_capacity(self,capacity):
        return f"{self.name}has a seating capacity of {capacity}."
        
        car = car("sedan", "Toyota", "Camry",2020,3000,4)
        print(car.sating_capacity(5))
        
        This outputs-
                     sedan has seating capacity of 5.
      
```


```python
For example - 
           
         class person:
            def __init__(self,name,age):
                self.name = name
                self.age = age 
                
            def display_person_info(self):
                print("Employee ID:", self.employee_id)
                print("salary:",self.salary)
                
         class Employee:
            def __init__(self,employee_id,salary):
                self.employee_id - employee_if
                self.salary = salary
                
            def display_employee_info(self):
                print("Employee ID:",self.employee_id)
                print("Salary:",self.salary)
                
    class Manager(person, Employee):
        def __init__(self,name,age,employee_id,salary,department):
            person.__init__(self,name,age)
            Employee.__init__(self, employee_id,salary)
            self.department = department
            
    def display_manager_info(self):
        person.display_person_info(self)
        employee.display_employee_info(self)
        print("Department:"self.department)
        
        manager = manager("john Doe",35,12345,50000,"IT")
        manager.display_manager_info()
        
    output- 
          Name: John Doe
          Age: 35
          Employee Id : 12345
          Department:IT

```


      Cell In[3], line 1
        For example -
            ^
    SyntaxError: invalid syntax




```python
4.What are getter and setter in python? create a class and create a getter and a setter method in this class.

Ana- 

   Getter and setter are method that allows you to access and modify the values of the private attributes of a class.
    
    In python, you can define getter and setter methds using the '@property' and '@<property_name>.setter' decorators,resp.
    for example- 
                 class Temperatur:
            def __init__self(self,temperature):
                self._temperature = temperature
                
             @property
              def temperature(self):
                    return self._temperature
             @temperature.setter
              def temperature(self,value):
                    if value< -273.15:
                        raise valueError("temperature below absolute zero")
                        self._temperature = value
                        
            temp = Temperature(20)
            print("Temperature:",temp.temperature)
            
            temp.temperature = 25
            print("Temperature:",temp.temperature)
            
            output:
                    Temperature:20
                    Temperature:25
            
                
                
    
    
```

5.what is method overriding in python? Write a python code to demonstrate method overriding.

Ans- 
    method overriding is a feature of object-oriented programing languages where a subclass can provide a new implement.
    
for example- 
          
           class shape:
            def area(self):
                pass
          
           class Rectanle(shape):
                def __init__(self,width,height):
                    self.width = width
                    self.height = height
                    
                def area(self):
                    return self.width = self.height
                
            class Circle(shape):
                def __init__(self,radius):
                    self.radius = radius
                
                def area(self):
                    return 3.14 = self.radius * self.radius
                
                react = Rectangle(10,20)
                print("Area of Rectangle:",react.area())
                
                circle = Circle(5)
                print("Area of Circle:",circle.area())
                
                
            output:
                   Area of Rectangle:200
                   Area of Circle:78.5
                
                    
                
                
