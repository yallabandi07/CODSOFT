# codsoft
# TASK2
# Calculator
import math

# Function to add two numbers
def add(x, y):
    return x + y

# Function to subtract two numbers
def subtract(x, y):
    return x - y

# Function to multiply two numbers
def multiply(x, y):
    return x * y

# Function to divide two numbers
def divide(x, y):
    if y == 0:
        return "Cannot divide by zero"
    return x / y

# Function for power
def power(x, y):
    return x ** y

# Function for square root
def square_root(x):
    if x < 0:
        return "Invalid input"
    return math.sqrt(x)

# Function for modulus
def modulus(x, y):
    if y == 0:
        return "Cannot divide by zero"
    return x % y

# Prompt the user for input
num1 = float(input("Enter first number: "))
num2 = float(input("Enter second number: "))

print("Choose an operation:")
print("1. Addition")
print("2. Subtraction")
print("3. Multiplication")
print("4. Division")
print("5. Power")
print("6. Square Root")
print("7. Modulus")

choice = input("Enter operation (1/2/3/4/5/6/7): ")

if choice == '1':
    result = add(num1, num2)
elif choice == '2':
    result = subtract(num1, num2)
elif choice == '3':
    result = multiply(num1, num2)
elif choice == '4':
    result = divide(num1, num2)
elif choice == '5':
    result = power(num1, num2)
elif choice == '6':
    result = square_root(num1)
elif choice == '7':
    result = modulus(num1, num2)
else:
    result = "Invalid input"

print("Result: ", result
