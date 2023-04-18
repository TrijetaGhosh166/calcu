# calcu
#calculator by python


class Calculator:
    def __init__(self):
        pass
        
    def add(self, a, b):
        return a + b
    
    def subtract(self, a, b):
        return a - b
    
    def multiply(self, a, b):
        return a * b
    
    def divide(self, a, b):
        if b == 0:
            return "Error: Division by zero"
        return a / b
    
    def remainder(self, a, b):
        return a % b
    
    def root(self, a):
        return a ** 2
    
    def sqrroot(self, a):
        return a ** (1/3)
    
    def cube(self, a):
        return a ** 3
    
    def average(self, a, b):
        return (a + b) / 2
    
    def factorial(self, a):
        if a == 0:
            return 1
        else:
            return a * self.factorial(a-1)
    
    def pi(self,a):
        return a*3.14159265359
    
    def log(self, a):
        if a <= 0:
            return "Error: Invalid input"
        else:
            return math.log(a)

         op = Calculator()
print("0 -->for exit !!!\n-->")

print("1> for addition\n")
print("2> for subtraction \n")
print("3> for multiplication\n")
print("4> for division\n")
print("5> for remainder\n")
print("6> for root root\n")
print("7> for sqrroot\n")
print("8> for cube\n")
print("9> for average\n")
print("10> for factorial\n")
print("11> for pi\n")
print("12> for log\n")

while True:
    choice = int(input("Enter the option \n"))
    
    if choice == 0:
        break
    
    num1 = float(input("Enter first number: "))
    num2 = float(input("Enter second number: "))    
        
    if choice == 1:
        print("Result: ", op.add(num1, num2))
    elif choice == 2:
        print("Result: ", op.subtract(num1, num2))
    elif choice == 3:
        print("Result: ", op.multiply(num1, num2))
    elif choice == 4:
        print("Result: ", op.divide(num1, num2))
    elif choice == 5:
        print("Result: ", op.remainder(num1, num2))
    elif choice == 6:
        print("Result: ", op.root(num1))
    elif choice == 7:
        print("Result: ", op.sqrroot(num1))   
    elif choice == 8:
        print("Result: ", op.cube(num1))
    elif choice == 9:
        print("Result: ", op.average(num1, num2))
    elif choice ==10:
         print("Result: ", op.factorial(num1))
    elif choice ==11:
         print("Result: ", op.pi(num1))
    elif choice ==12:
         print("Result: ", op.log(num1))
                          
