def calculator():
    try:
        num1 = float(input("Enter first number: "))
        num2 = float(input("Enter second number: "))
        ope = input("Enter operation (+, -, *, /): ")

        if ope == '+':
            result = num1 + num2
            print(f"{num1} + {num2} = {result}")
        elif ope == '-':  # Changed 'operation' to 'ope'
            result = num1 - num2
            print(f"{num1} - {num2} = {result}")
        elif ope == '*':
            result = num1 * num2
            print(f"{num1} * {num2} = {result}")
        elif ope == '/':
            if num2 == 0:
                print("Error: Division by zero is not allowed.")
            else:
                result = num1 / num2
                print(f"{num1} / {num2} = {result}")
        else:
            print("Invalid operation. Please enter +, -, *, or /.")

    except ValueError:
        print("Invalid input. Please enter numerical values.")

calculator()
