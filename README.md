import math

def add(x,y):
  return x+y

def multiply(x,y):
  return x*y

def subtract(x,y):
  return x-y

def divide(x,y):
  if y==0:
    return "Math Error"
    return x/y

def power(x,y):
  return x**y

while True:
  print("Options:")
  print("Enter 'add' for addition")
  print("Enter 'subtract' fir subtraction")
  print("Enter 'multiply' for multiplicaton")
  print("Enter 'power' for exponentiation")
  print("Enter 'quit' to exit the program")

  user_input = input(": ")

  if user_input == "quit" :
    break
  elif user_input in ["add", "subtract", "multiply", "divide", "power"]:
    num1= float(input("Enter first digit:"))
    num2= float(input("Enter second digit:"))

    if user_input == "add":
      print("Result: ", add(num1, num2))
    elif user_input == "subtract":
      print("Result: ", subtract(num1, num2))
    elif user_input == "multiply":
      print("Result: ", multiply(num1, num2))
    elif user_input == "divide":
      print("Result: ", divide(num1, num2))
    elif user_input == "power":
      print("Result: ", power(num1, num2))

    else:
      print("Invalid input.")
