# OOP-Coffee-Machine-Program
This project simulates a coffee machine using Object-Oriented Programming (OOP) in Python. Users can purchase coffee drinks like espresso, latte, or cappuccino, and the machine keeps track of resources (water, milk, coffee), processes payments via coins, and manages the order flow for multiple coffee drinks.

# Project Structure
The project is organized into four Python files, each representing a key object in the OOP architecture:

``` 1. coffee_maker.py ```

Class: ``` CoffeeMaker ```

**Responsibilities:**
- Manages and stores the coffee machine's resources (water, milk, coffee).
- Provides methods to check if enough resources are available for a drink order.
- Updates the resources after a drink is made.
- Prints a report of current resources for the user.

``` 2. menu.py ```

Classes: ``` Menu, MenuItem ```

**Responsibilities:**
- **MenuItem:** Represents a single coffee drink as an object, including its ingredients (water, milk, coffee) and its cost.
- **Menu:** Acts as a collection of available MenuItem objects. It provides methods to retrieve available drinks and search for a drink by name.

``` 3. money_machine.py ```

Class: ``` MoneyMachine ```

**Responsibilities:**
- Handles the machine’s coin-based payment system.
- Processes user coin input, calculates the total amount of money received, and checks if the payment is sufficient.
- Tracks profits and returns change or refunds as needed.
- Prints a report of current profits.

``` 4. main.py ```

**Responsibilities:**
- Acts as the control interface for the coffee machine, integrating the CoffeeMaker, Menu, and MoneyMachine classes.
- Manages user input and allows the user to:
   - Select a drink from the menu.
   - Insert coins to make payments.
   - Get reports on available resources and profit.
- Checks if there are enough resources for a drink and if the user has inserted sufficient money before completing the order.

---

# Features:
- **Drink Selection:** User selects a drink (espresso, latte, or cappuccino) from the Menu.
- **Resource Management:** The CoffeeMaker class manages the water, milk, and coffee levels.
- **Coin Payment System:** The MoneyMachine class simulates the insertion of coins (quarters, dimes, nickels, pennies).
- **Profit Reporting:** The MoneyMachine class tracks and displays the total profit earned by the machine.
- **Error Handling:**
  - The CoffeeMaker checks if there are enough resources before making a drink.
  - The MoneyMachine checks if enough money has been inserted and returns change or refunds payment if necessary.
 
# Notes
* **Design:** Each class (CoffeeMaker, Menu, MenuItem, MoneyMachine) has its own clear responsibility, ensuring modular and reusable code.
* **Encapsulation:** By using OOP, each part of the system (coffee resources, menu, and money processing) is encapsulated within its own class, making the code easier to maintain and extend.
* **Scalability:** New drinks can be added easily by extending the Menu class, demonstrating the flexibility of the OOP structure.
