
def add(x, y):
    return x + y

def subtract(x, y):
    return x - y

def multiply(x, y):
    return x * y

def divide(x, y):
    if y != 0:
        return x / y
    else:
        return "Cannot divide by zero"

# Input from the user
num1 = float(input("Enter the first number: "))
num2 = float(input("Enter the second number: "))

# Display the available operations
print("\nChoose operation:")
print("1. Addition (+)")
print("2. Subtraction (-)")
print("3. Multiplication (*)")
print("4. Division (/)")

# Input the operation choice
operation = input("Enter the operation number (1, 2, 3, or 4): ")

# Perform the calculation based on the operation choice
if operation == "1":
    result = add(num1, num2)
    operator = "+"
elif operation == "2":
    result = subtract(num1, num2)
    operator = "-"
elif operation == "3":
    result = multiply(num1, num2)
    operator = "*"
elif operation == "4":
    result = divide(num1, num2)
    operator = "/"
else:
    print("Invalid operation choice")
    exit()

# Display the result
print(f"\nResult: {num1} {operator} {num2} = {result}")
