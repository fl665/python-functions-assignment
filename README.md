# python-functions-assignment

1.Create a function named calculate_discount(price, discount_percent) that calculates the final price after applying a discount. The function should take the original price (price) and the discount percentage (discount_percent) as parameters. If the discount is 20% or higher, apply the discount; otherwise, return the original price.

def calculate_discount(price, discount_percent):
    # Check if the discount is 20% or higher
    if discount_percent >= 20:
        # Apply the discount
        final_price = price * (1 - discount_percent / 100)
        return final_price
    else:
        # Return the original price if the discount is less than 20%
        return price

2.Using the calculate_discount function, prompt the user to enter the original price of an item and the discount percentage. Print the final price after applying the discount, or if no discount was applied, print the original price.

def calculate_discount(price, discount_percent):
    # Check if the discount is 20% or higher
    if discount_percent >= 20:
        # Apply the discount
        final_price = price * (1 - discount_percent / 100)
        return final_price
    else:
        # Return the original price if the discount is less than 20%
        return price

# Prompt the user for input
price = float(input("Enter the original price of the item: "))
discount_percent = float(input("Enter the discount percentage: "))

# Calculate the final price
final_price = calculate_discount(price, discount_percent)

# Print the result
if final_price == price:
    print(f"No discount applied. The original price is: {price}")
else:
    print(f"Final price after {discount_percent}% discount: {final_price}")
