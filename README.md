def calculator():
    print("Simple Calculator")
    print("Operations: + (Addition), - (Subtraction), * (Multiplication), / (Division)")

    # Input numbers
    num1 = float(input("Enter first number: "))
    num2 = float(input("Enter second number: "))

    # Input operation
    operation = input("Enter operation (+, -, *, /): ")

    # Perform operation
    if operation == '+':
        result = num1 + num2
        print(f"Result: {num1} + {num2} = {result}")
    elif operation == '-':
        result = num1 - num2
        print(f"Result: {num1} - {num2} = {result}")
    elif operation == '*':
        result = num1 * num2
        print(f"Result: {num1} * {num2} = {result}")
    elif operation == '/':
        if num2 != 0:
            result = num1 / num2
            print(f"Result: {num1} / {num2} = {result}")
        else:
            print("Error: Cannot divide by zero.")
    else:
        print("Invalid operation. Please choose +, -, *, or /")

# Run the calculator
calculator()
