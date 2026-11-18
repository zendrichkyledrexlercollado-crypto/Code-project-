# Code-project-# ==========================================
# PYTHON TUTORIAL PROGRAM - Beginner to Pro
# Run this file and follow along!
# ==========================================

print("Welcome to Python Tutorial!")
print("=" * 40)

# 1. VARIABLES & DATA TYPES
print("\n1. VARIABLES & DATA TYPES")
name = "Kyle"
age = 20
height = 5.8
is_student = True

print(f"Name: {name} - type: {type(name)}")
print(f"Age: {age} - type: {type(age)}")
print(f"Height: {height} - type: {type(height)}")
print(f"Is Student: {is_student} - type: {type(is_student)}")

# 2. USER INPUT
print("\n2. USER INPUT")
# Uncomment to try it live:
# user_name = input("What is your name? ")
# print(f"Hello, {user_name}!")

# 3. MATH OPERATORS
print("\n3. MATH OPERATORS")
a = 10
b = 3
print(f"{a} + {b} = {a + b}")
print(f"{a} - {b} = {a - b}")
print(f"{a} * {b} = {a * b}")
print(f"{a} / {b} = {a / b}")
print(f"{a} // {b} = {a // b}  (floor division)")
print(f"{a} % {b} = {a % b}  (remainder)")
print(f"{a} ** {b} = {a ** b}  (power)")

# 4. IF / ELSE - DECISIONS
print("\n4. IF / ELSE")
score = 85
if score >= 90:
    print("Grade: A")
elif score >= 80:
    print("Grade: B")
elif score >= 70:
    print("Grade: C")
else:
    print("Grade: F")

# 5. LOOPS
print("\n5. FOR LOOP")
for i in range(1, 6):
    print(f"Count: {i}")

print("\n6. WHILE LOOP")
count = 1
while count <= 3:
    print(f"While count: {count}")
    count += 1

# 7. LISTS
print("\n7. LISTS")
fruits = ["apple", "banana", "mango", "orange"]
print(f"My fruits: {fruits}")
print(f"First fruit: {fruits[0]}")
print(f"Last fruit: {fruits[-1]}")

fruits.append("grapes")
print(f"After adding: {fruits}")

for fruit in fruits:
    print(f"- I like {fruit}")

# 8. DICTIONARIES
print("\n8. DICTIONARIES")
student = {
    "name": "Kyle",
    "age": 20,
    "course": "BSIT",
    "city": "Mabalacat"
}
print(student)
print(f"Name: {student['name']}")
print(f"Course: {student['course']}")

# 9. FUNCTIONS
print("\n9. FUNCTIONS")

def greet(name):
    return f"Hello, {name}! Welcome to Python."

def add_numbers(x, y):
    return x + y

def calculator(num1, num2, operation):
    if operation == "+":
        return num1 + num2
    elif operation == "-":
        return num1 - num2
    elif operation == "*":
        return num1 * num2
    elif operation == "/":
        return num1 / num2 if num2 != 0 else "Cannot divide by zero"
    else:
        return "Invalid operation"

print(greet("Kyle"))
print(f"5 + 7 = {add_numbers(5, 7)}")
print(f"Calculator: 10 * 5 = {calculator(10, 5, '*')}")

# 10. MINI PROJECT: SIMPLE CALCULATOR + QUIZ
print("\n10. MINI PROJECT: NUMBER GUESSING GAME")
import random

def guessing_game():
    secret = random.randint(1, 10)
    print("I'm thinking of a number between 1 and 10...")
    # Uncomment to play:
    # for attempt in range(3):
    #     guess = int(input(f"Attempt {attempt+1}/3 - Your guess: "))
    #     if guess == secret:
    #         print("Correct! You win!")
    #         return
    #     elif guess < secret:
    #         print("Too low!")
    #     else:
    #         print("Too high!")
    # print(f"Game over! The number was {secret}")

    print(f"[Demo] Secret number was: {secret} - uncomment the code above to play!")

guessing_game()

print("\n" + "=" * 40)
print("Tutorial Complete! Great job!")
print("Next to learn: Classes, Files, APIs, and Web Development")