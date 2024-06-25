
# Coffee Machine Program

This is a simple coffee machine program written in Python. It allows the user to order coffee, process payments, and manage resources for making different types of coffee drinks.

## Features

- **Order Coffee**: Choose from three types of coffee: espresso, latte, and cappuccino.
- **Check Resources**: Ensure there are enough ingredients to make the selected coffee.
- **Process Payments**: Insert coins to pay for the coffee.
- **Transaction Handling**: Check if the payment is sufficient and return change if necessary.
- **Update Resources**: Deduct the required ingredients from the machine's resources after making a coffee.
- **Reporting**: Display the current resources and profit.

## Menu

- **Espresso**
  - Ingredients: 50ml water, 18g coffee
  - Cost: $1.5
- **Latte**
  - Ingredients: 200ml water, 150ml milk, 24g coffee
  - Cost: $2.5
- **Cappuccino**
  - Ingredients: 250ml water, 100ml milk, 24g coffee
  - Cost: $3.0

## Resources

- Water: 300ml
- Milk: 200ml
- Coffee: 100g

## Usage

1. **Start the Machine**: Run the program.
2. **Select an Option**: Choose between ordering a coffee (`espresso`, `latte`, `cappuccino`), viewing the report (`report`), or turning off the machine (`off`).
3. **Order Coffee**: When prompted, select the type of coffee you want.
4. **Check Resources**: The program will check if there are enough ingredients to make the selected coffee.
5. **Insert Coins**: If there are enough resources, the program will prompt you to insert coins.
6. **Transaction Handling**: The program will check if the inserted coins are sufficient to cover the cost. If so, it will make the coffee and provide change if necessary. If not, it will refund the money.
7. **Receive Coffee**: Enjoy your coffee!

## Functions

- **is_resource_sufficient(order_ingredients)**: Checks if there are enough resources to make the selected coffee.
- **process_coins()**: Processes the coins inserted by the user and returns the total amount.
- **is_transaction_successful(money_received, drink_cost)**: Checks if the inserted money is sufficient and handles the transaction.
- **make_coffee(drink_name, order_ingredients)**: Deducts the required ingredients from the resources and makes the coffee.

## Example

```python
$ python coffee_machine.py
What would you like? (espresso/latte/cappuccino): latte
Please insert coins.
how many quarters?: 10
how many dimes?: 0
how many nickles?: 0
how many pennies?: 0
Here is $0.0 in change.
Here is your latte ☕️. Enjoy!
```

## Notes

- Ensure to keep the resources updated to reflect the real machine's status.
- The program will continue to run until the user inputs `off`.
- Use the `report` option to check the remaining resources and profit at any time.

---
