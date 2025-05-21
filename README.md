# Calculator_in_Python
A simple Python calculator program that performs basic arithmetic operations (addition, subtraction, multiplication, and division). The program asks the user to input an operator (+, -, *, /) and two numbers, and it calculates the result.

```python

try:
    operator = input("Enter an operator (+ - / * ): ")
    num1 = float(input("Enter the first number: "))
    num2 = float(input("Enter the second number: "))
    if operator == "+":
        result = num1 + num2
        print(round(result, 3))
    elif operator == "-":
        result = num1 - num2
        print(round(result, 3))
    elif operator == "/":
        result = num1 / num2
        print(round(result, 3))
    elif operator == "*":
        result = num1 * num2
        print(round(result, 3))
    else:
        print(f'{operator} is not a valid operator.')
except ValueError:
    print("Invalid input. Please enter a valid number.")
