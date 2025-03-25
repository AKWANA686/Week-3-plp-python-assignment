## Week 3 Assignment

This is a PLP PYTHON WEEK 3 ASSIGNMENT meant to test our understandability on loops and functions.

1. Create a function named calculate_discount(price, discount_percent) that calculates the final price after applying a discount. The function should take the original price (price) and the discount percentage (discount_percent) as parameters. If the discount is 20% or higher, apply the discount; otherwise, return the original price.

def calculate_discount(price, discount_percent):
if discount_percent >= 20:
discount_amount = (price \* discount_percent) / 100
final_price = price - discount_amount
return final_price
else:
return price

Using the calculate_discount function, prompt the user to enter the original price of an item and the discount percentage. Print the final price after applying the discount, or if no discount was applied, print the original price.

# Get user input

price = float(input("Enter the original price of the item: "))
discount_percent = float(input("Enter the discount percentage: "))

#Call the function with user input
final_price = calculate_discount(price, discount_percent)

#Print the result
if discount_percent >= 20:
print(f"Discount applied. Final price: ${final_price}")
else:
print(f"No discount applied. Price remains: ${final_price}")
