# the-tuff-calculator
#its a calculator with a tuff twist


import time

print ("[1] for addition")
print ("[2] for subtraction")
print ("[3] for multiplication")
print ("[4] for division")

choice = input("Enter your choice (1/2/3/4/5): ")

if choice == "1":
    num1 = int(input("Enter your first number: "))
    num2 = int(input("Enter your second number: "))
    confirm = input("Are you ready to calculate your result? (y/n): ")
    if confirm == "y":
        print(num1 + num2)
    if confirm == "n":
        print ("Okay calculation cancelled")

if choice == "2":
    num1 = int(input("Enter your first number: "))
    num2 = int(input("Enter your second number: "))
    confirm = input("Are you ready to calculate your result? (y/n): ")
    if confirm == "y":
        print(num1 - num2)
    if confirm == "n":
        print ("Okay calculation cancelled")

if choice == "3":
    num1 = int(input("Enter your first number: "))
    num2 = int(input("Enter your second number: "))
    confirm = input("Are you ready to calculate your result? (y/n): ")
    if confirm == "y":
        print(num1 * num2)
    if confirm == "n":
        print ("Okay calculation cancelled")

if choice == "4":
    num1 = int(input("Enter your first number: "))
    num2 = int(input("Enter your second number: "))
    confirm = input("Are you ready to calculate your result? (y/n): ")
    if confirm == "y":
        print(num1 / num2)
    if confirm == "n":
        print ("Okay calculation cancelled")

if choice == "5":
    tuff = input("What is 32 + 35: ")
    if tuff == "67":
        for _ in range(67):
            print (32 + 35)
            time.sleep (0.2)
