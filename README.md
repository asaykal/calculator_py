# Calculator

This is a simple calculator program written in Python. It is my Day 1 project for the Python Confidence Builder collection.

```python
class Calculator:
    
    def __init__(self, var_1, var_2):  
        
        self.var_1 = var_1
        self.var_2 = var_2
    
    def aggregation(self):  
        result = self.var_1 + self.var_2
        return result

    def subtraction(self): 
        result = self.var_1 - self.var_2
        return result

    def multiplaction(self): 
        result = self.var_1 * self.var_2
        return result
    
    def division(self):    
        result = self.var_1 / self.var_2
        return result

try :
    
    print
    ("""
    █▀▀ ▄▀█ █░░ █▀▀ █░█ █░░ ▄▀█ ▀█▀ █▀█ █▀█
    █▄▄ █▀█ █▄▄ █▄▄ █▄█ █▄▄ █▀█ ░█░ █▄█ █▀▄
    """)

    while True:
        var_1 = int(input("First Number : "))
        var_2 = int(input("Second Number : "))
        
        operator = input("Which operation do you want to perform? : ")
        
        result = None
        Calculator = Calculator(var_1, var_2)
        
        if operator == "+":
            result = Calculator.aggregation()
            
        if operator == "-":
            result = Calculator.subtraction()
        
        if operator == "*":
            result = Calculator.multiplaction()
        
        if operator == "/":
            result = Calculator.division()
            
        if var_1 == "e" or var_2 == "e" or operator == "e":
            exit()
            
        print("Result : ", result)
        print("Enter 'e' to exit.")
        

except :
    
    print("Error")

```

## Features
- Addition, subtraction, multiplication, and division operations
- Simple user interface
- Basic error handling (e.g. division by zero)

### TO-DO

In future versions of this program, I plan to add more advanced features such as exponentiation, square roots, and trigonometric functions. I also plan to improve the user interface and add more sophisticated error handling. 
