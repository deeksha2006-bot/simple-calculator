def calculator():
    print("🧮 Welcome to Python Calculator 🧮")
    print("Operations: +  -  *  /")

    while True:
        num1 = float(input("\nEnter first number: "))
        op = input("Enter operation (+, -, *, /): ")
        num2 = float(input("Enter second number: "))

        if op == "+":
            print("Result =", num1 + num2)
        elif op == "-":
            print("Result =", num1 - num2)
        elif op == "*":
            print("Result =", num1 * num2)
        elif op == "/":
            if num2 != 0:
                print("Result =", num1 / num2)
            else:
                print("❌ Error! Division by zero.")
        else:
            print("❌ Invalid operation!")

        choice = input("\nDo you want to continue? (y/n): ")
        if choice.lower() != "y":
            print("Goodbye! 👋")
            break

# Run the calculator
calculator()

