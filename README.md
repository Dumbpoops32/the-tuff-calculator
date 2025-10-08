# the-tuff-calculator
#its a calculator with a tuff twist


import time

def calculate(a, b, operation):
    if operation == "1":
        return a + b
    elif operation == "2":
        return a - b
    elif operation == "3":
        return a * b
    elif operation == "4":
        return a / b

def main():
    print("[1] Addition")
    print("[2] Subtraction")
    print("[3] Multiplication")
    print("[4] Division")
    print("[5] Special Challenge")

    choice = input("Enter your choice (1/2/3/4/5): ")

    if choice in ["1", "2", "3", "4"]:
        try:
            num1 = float(input("Enter your first number: "))
            num2 = float(input("Enter your second number: "))
        except ValueError:
            print("Invalid input. Please enter a number.")
            return
        
        confirm = input("Are you ready to calculate your result? (y/n): ").lower()
        if confirm == "y":
            result = calculate(num1, num2, choice)
            print(f"Result: {result}")
        else:
            print("Calculation cancelled.")

    elif choice == "5":
        tuff = input("What is 32 + 35: ")
        if tuff == "67":
            for _ in range(67):
                print(67)
                time.sleep(0.2)
        else:
            print("Incorrect! Try again next time.")

    else:
        print("Invalid choice. Please select 1, 2, 3, 4, or 5.")

if __name__ == "__main__":
    main()
