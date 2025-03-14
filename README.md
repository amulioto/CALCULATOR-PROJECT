# CALCULATOR-PROJECT
# Simple calculator program
def calculate(num1, num2, operation):
    if operation == "+":
        return num1 + num2
    elif operation == "-":
        return num1 - num2
    elif operation == "*":
        return num1 * num2
    elif operation == "/":
        if num2 == 0:
            return "Error: Division by zero is not allowed."
        return num1 / num2
    else:
        return "invalid operation"

# Get user input
num1 = float(input("Enter first number: "))
num2 = float(input("Enter second number:"))
operation = input("Enter operation (+, -, *, /): ")

# Perform calculation and print the result
result = calculate(num1, num2, operation)
print("The result is:", result)
