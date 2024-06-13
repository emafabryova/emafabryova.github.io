def calculator(typeAction, firstNumber, secondNumber):
    if typeAction not in "+ - * /":
        return ("Wrong input.")
    if typeAction == "+":
        return (firstNumber + secondNumber)
    elif typeAction == "-":
        return(firstNumber - secondNumber)
    elif typeAction == "*":
        return(firstNumber * secondNumber)
    elif typeAction == "/":
        return(firstNumber/secondNumber)

while True: 
    typeAction = input("Choose: +, -, *, /." )
    if typeAction not in "+ - * /":
        print("Enter valid input.")
    else:
        firstNumber = int(input("Enter your first number: "))
        secondNumber = int(input("Enter your second number: "))
        print (calculator(typeAction, firstNumber, secondNumber))
