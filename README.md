.

🛒 Python Shopping Cart Program

This Python program simulates a simple shopping cart system using lists.

Users can:

Add food items

Enter their prices

Quit when finished

View all items

See the total cost

📄 File Structure
main.py
README.md

🚀 What This Program Does

Continuously asks the user to enter food items

Stops when the user types q

Stores:

Item names in one list

Prices in another list

Calculates and displays the total price

🛠️ How It Works

foods = [] → stores item names

prices = [] → stores item prices

while True loop → keeps asking until user quits

append() → adds items to lists

A for loop sums all prices

The final total is displayed using formatted output

📄 Code Example
foods = []
prices = []
total = 0

while True:
    food = input("Enter a food to buy (q to quit):")
    if food.lower() == "q":
        break
    else:
        price = float(input(f"Enter the price of a {food}: $"))
        foods.append(food)
        prices.append(price)

print("-----YOUR CART -----")

for food in foods:
    print(food, end=' ')

for price in prices:
    total += price

print(f"Your Total Is ${total}")

▶️ How to Run

Make sure Python is installed

Open a terminal in the project folder

Run:

python main.py

📌 Example Output
Enter a food to buy (q to quit): Apple
Enter the price of a Apple: $2.5
Enter a food to buy (q to quit): Bread
Enter the price of a Bread: $3
Enter a food to buy (q to quit): q
-----YOUR CART -----
Apple Bread
Your Total Is $5.5

🎯 Learning Objectives

This project helps practice:

Lists

While loops

Conditional statements

Appending to lists

Summing values

Basic program structure
