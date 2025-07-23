# Calculator
Created my first calculator.
def add(n1,n2):
    return n1+n2
def subtract(n1,n2):
    return n1-n2
def multiply(n1,n2):
    return n1*n2
def divide(n1,n2):
    return n1/n2 

     

n1 = int(input("Enter first number: "))
is_continue = True
while is_continue:
    operation = input("enter you operation  (+ , _ , * , /) : ")
    n2 = int(input("Enter your second number : "))
    if operation == "+":
        result = add(n1,n2)
    if operation == "-":
        result = subtract(n1,n2)    
    if operation == "*":
        result = multiply(n1,n2)
    if operation == "/":
        result = divide(n1,n2) 
    else:
        print("invalid operation")
    print(f" result: {result}") 
    more = input("do you want to continue?: ").lower()
    if more == "yes":
        n1 = result
    else:
        is_continue = False

    
