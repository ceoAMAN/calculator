def calculator():
    def select_opreation(*args):
        return "Select operation: " + ", ".join(args) + ": "
    
    print("Welcome to the calculator")
    print("Enter two numbers to perform operations")
    print("You can perform operations like +, -, /, *, **, //, %")  
    
    x = int(input("Enter number: "))
    y = int(input("Enter number 2: "))
    select = input(select_opreation("+", "-", "/", "*", "**", "//", "%"))
    
    if select == "+":
        print(x + y)
    elif select == "-":
        print(x - y)
    elif select == "/":
        print(x / y)
    elif select == "*":
        print(x * y)
    elif select == "**":
        print(x ** y)
    elif select == "//":
        print(x // y)
    elif select == "%":
        print(x % y)
    else:
        print("Invalid operation")

calculator()
print("Thank you for using the calculator")
do_you_want_to_reuse = input("do you want to use again? (yes/no): ")
if  do_you_want_to_reuse == "yes":
    calculator()
else:
    do_you_want_to_reuse == "no"
    print("Thank you for using the calculator")
